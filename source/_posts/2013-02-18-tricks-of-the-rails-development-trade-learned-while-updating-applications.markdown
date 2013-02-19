---
layout: post
title: "Tricks of the Rails Development Trade learned while updating applications"
date: 2013-02-18 10:02
comments: true
categories: 
---


As I'm sure most of us are aware, rails recently had some security holes brought to light and fixed.

These are my notes after upgrading about a dozen applications, many of them twice in the past month or two.

If you don't have a solid batch of unit tests, then the odds of my spending anytime on patching your open source project are nil. Well, not quiet. I've done a few.

But seriously, with tests, my workflow looks something like this:

  - read README. Make note of any special dependencies, like elasticsearch or postgres in development.

  - git clone.

  - create new rvm gemset.

  - `bundle install`.

  - read through `config/database.yml`, change if needed to work with my setup. Changes are normally limited to things like the database name, the database user, password, etc. 

  - `rake db:create`
  - `rake db:migrate && rake db:seed && rake db:test:prepare`

  - and then I run the tests - either `rake test`, `rspec spec` or `rake spec`. I've seen all three of them, and I'm sure I'll see more variations as time goes on. Side note: For rails applications, we should always alias `rake test` to the testing framework that is being used.

  - if the tests all pass before I upgrade, I upgrade with `bundle update rails && rake test`, if they don't, then I try to make them pass (I normally can), but if I can't, I and then update rails, re-run the tests, and make sure they are either all green, or that there are no new failures. (No more than 5% of the tests can fail).
  
  - commit, submit a pull request, ping the maintainer on twitter after 24 hours 
  if it isn't merged.

Without tests:

- git clone
- `bundle install`
- `rake db:migrate`
- `rails server`
- poke around in the browser.
- `update rails`
- spend my time going through weird stacktaces and weird errors, or worse, not knowing if I broke something. 

Ew.


So, the take aways are:

- Documentation on how to get a fully functional dev environment, having tests, and having the code on github. 

- Test suites rule.

- Readable code is also important - there were a few situations where the tests were failing, and I had to go through and read the code to understand *why*, and it was surprisingly easy to debug these applications - I'm sure that the test-driven design was also a big part of it, but there was also a certain element of "this is readable code, I can understand this". 

Oh, and if you're looking for someone to update your rails applications with critical security fixes in the future, [lets talk](http://jamesrgifford.com/contact). 