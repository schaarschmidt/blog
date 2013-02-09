---
layout: post
title: "Nexus 7: A Worthy Tool for the System Administrator"
date: 2013-02-09 09:12
comments: true
categories: ubuntu-planet
---

The last day of August, 2012, I got a box in the mail. The contents? A 16GB Nexus 7. My first android device.

Since then, its been a fun ride, and I've learned the various cool tools out there for a IT person.

I do contract work with a nameless startup incubator in the area, and as part of that, I'm partially responsible for printers, user-facing documentation, etc.

As such, I was constantly plugging and unplugging my laptop to show people this, that or the other. *however*, the tablet has replaced my laptop for a lot of those duties. Let me explain more.


### Documentation.

Like it or not, we all have to document things. And we have to do it well, for our intended audience. Now, we have two main pieces of user-facing documentation - the WiFi setup, and the printer setup. Two documents,one of which changes as we fix things (printers).

The Nexus 7 is just the right for me to pull of the document and refer to it as I'm working on someone's machine. The apps I use for that are:

- Dropbox. We use a shared dropbox folder to share the documents.

Now, to view them, I need a office type tool. While I could (and have) use Google drive, it doesn't lend itself to the situation well.

I've looked at the softmaker line of products, but I haven't been impressed with their linux offerings, so I'm not sure if I should risk the price for the full amount.


However, I am very happy with Kingston Office Writer.


![](http://i.imgur.com/5FvPpyWh.png)

![](http://i.imgur.com/4PHiEUlh.png)


It's free, and available for Android [here](https://play.google.com/store/apps/details?id=cn.wps.moffice_eng).


### SSH.

The ConnectBot family is well-known and very well featured for being able to do SSH.

However, [I've discovered that stock ConnectBot doesn't play nice with function keys](http://code.google.com/p/connectbot/issues/detail?id=369) on bluetooth keyboards, so I am using a fork of ConnectBot called [VX ConnectBot](https://play.google.com/store/apps/details?id=sk.vx.connectbot) that properly supports external keyboards.

ConnectBot supports SSH keys, although I don't make use of them  - I don't do enough SSH on my tablet to worry about that.


### Notes.


Evernote. [While I used to be a fan of Tomboy/Tomdroid/Ubuntu One](http://blog.jamesrgifford.com/dropbox-to-ubuntu-one-for-note-taking/), recent events have pushed me into the Evernote fold. And I must say, it's nice. I'm using it to write this blog post right now.


I shell out the cash each month for Evernote Premium, and while I'm enjoying it so far, there are a few "problems" I have with it, but I also had them with Tomboy.

- No [Markdown](http://daringfireball.net/projects/markdown/) support. Really, everything should support markdown.
- Search sucks. Always has, always will. Someday someone will make search that doesn't suck, but that day has not yet come.
- inline image embedding. For this, that'd be really nice. But oh well.


### PDF Viewer.

[Amazon Kindle](https://play.google.com/store/apps/details?id=com.amazon.kindle) or the built-in PDF reader are my go-to PDF readers. They aren't terrific, but they are ok.

### Email.

Ahg. Email, the bane of every IT persons existence. Email is something I detest.
People need to understand that when they email me, I will see it, and then prioritize it. I'm sad that people think that emailing me = instant response and I go and fix their problem. If you email someone, you should expect up to a 72 hour wait period before you get a response. If it's that important, call me. The important people have my number, and the smart ones who might need to call me know where and how to find it.

Anyway, I use the excellent gmail app for my email. I have gmail filters setup server side that filter out mailing lists and similar things into gmail tags, so they never hit my inbox. I then have gmail setup to only send me a push notification if it's in the priority inbox.

![](http://i.imgur.com/JHwDDdf.jpg)

So, lets bits and pieces that don't really fall into any category are:

More communication tools: [Skype](https://play.google.com/store/apps/details?id=com.skype.raider) , Google Talk (no link that I could find in the Play Store) and for IRC, I'm a fan of [AndChat(https://play.google.com/store/apps/details?id=net.andchat). [Google Voice](https://play.google.com/store/apps/details?id=com.google.android.apps.googlevoice) is another good one, if you're a Google Voice user, I highly recommend installing the application - while I still haven't figured out how to make calls from my Nexus 7, for text messages, it works fine. Lastly, for those times that Skype is just being a pain in the rear, there is Google + Hangouts, which are pretty useful.


### Web Browser

For choice of Browser, I have two installed. I have [Chrome Beta](https://play.google.com/store/apps/details?id=com.chrome.beta), and I have [Firefox](https://play.google.com/store/apps/details?id=org.mozilla.firefox). My main browser is Chrome, and I have Firefox for accessing all the internal sites that require self-signed SSL certificates. I much prefer Chromes tab setup, but Firefox is pretty fast.


### Password management:

I'm cheap, remember? So I am a fan of [keepass](http://keepass.info) and Dropbox.

So I store my passwords in a Keepass2 (or KeepassX) database, synced to my Dropbox folder. On my Tablet, I use keepassdroid to access it, and it's all hunky dory.

Other tools I've tried are:

- [Universal Password Manager](http://upm.sourceforge.net). I can't explain why, but something about it not being in the archive for Ubuntu just made me not want to deal with it.

- [LastPass](https://lastpass.com/). Only way to get the mobile apps is the give them money, and I'm not a fan of proprietary applications storing something like my passwords. At least in dropbox, everything is a file.


### Todo list:

I use a combination of [todo.txt](http://todotxt.com/) and [Wunderlist](http://wunderlist.com/), but I'm not entirely sure how well it's working. Ask me in a few months.

So, that's my list of tools. What is in your toolbox?

