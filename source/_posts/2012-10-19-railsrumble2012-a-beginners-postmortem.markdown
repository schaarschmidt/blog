---
layout: post
title: "RailsRumble 2012: A Beginners Postmortem"
date: 2012-10-19 18:46
comments: true
categories: ubuntu-planet
---

I thought I was a fairly competent and accomplished rails developer, for someone who was self taught, never had a job doing rails stuff, and who was young enough that a large part of the community is old enough be my dad.


And then I entered the Rails Rumble for 2012 with [@imnotanerd](https://twitter.com/imnotanerd), and spent a desperate 48 hours with my battling oauth, rails internals, Sinatra, cancan, and a Linux server. 

At the end, I've got a few takeaways. 

- Come up with two ideas - one that only takes 12 hours to build, the other that takes the full 48. 

  This saved our bacon. We had two ideas - one was fairly complex. At 8PM Saturday I said "look. We've been banging our heads against this for almost 8 man hours. Time to start something else."

  So I did a rails new, and thus Volla was born. Or reborn. 

- Git is your frenemy. 

  Git is a blessing and a curse. Commit early, often, push, deploy via Capistrano, repeat. 

  But make sure that your gitignore is properly updated. 

  Otherwise, you end up committing 20mb worth of binstubs. And your api keys. Not OK. 

  Anyway. Don't do that. 

- Stay on target... 

  Enough said. Don't get distracted by the cool matrix cat or something. 

- If you don't succeed, try again.
  Take a month off, then try that idea again. I learned everything I know about rails because I said "I've got two weeks. Let's building something in 2 hours a day". (Side note: that's how I got sucked into Shoes/Hackety Hack, as well as delayed_paperclip. You devote time to something, you will fill it. Fact of life that I've discovered over the past 16 years I've been around on this planet.)


- Leverage the knowledge of others.

  I did the math, and between the two of us, we spent 8 hours man hours trying to figure out sessions in Sinatra. It was at this point I said "stop and move on, lets get this fixed". Time spent on authentication in rails? 20 minutes. (Authorization though, was closer to an hour, hour and a half)


  The lesson to take away from this is that for almost everything you're doing, someone has invented that wheel already - so for the love of pete, USE IT. Thats the wonderful thing about a community.

- If you don't know what adding $GEM to your gemfile will do, you probably don't want to do it.

  I ran into this - had a gem, added it, broke everything. Removed, worked fine. (Not naming names here, it was some bad code I wrote elsewhere). But adding *one* gem was enough to break the whole app. 

- Use a logged chat. 

  We used skype - this worked, but the logs in skype are... well, less than wonderful. Part of this has to do with Skype for Linux, part of this has to do with Skype in general. If I had to do it again, I'd use Campfire, or even IRC. 

- Descriptive git commits. 

  "Fixed bugs" - If you're guilty of this, raise your hand! Oh look, everyones hand went up. 

  Don't. Do. This. Ever. Makes code review after the fact hard. 

- If you're confident, do some sort of TDD.

  This would have cost us time, but saved us trouble. If we had automated testing in place, I would have known that we broke certain things with certain other changes. But... well, hindsight is 20-20.

Hopefully my tips here will be useful for people in the future. If not, oh well. I tried. :)

