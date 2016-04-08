---
layout: post
category: post
"splash-tall": ""
"splash-wide": "/images/1-AeFmAZTEGrX_nTCpUdKJqQ.jpeg"
tags: 
  - "null"
published: true
title: Chat Interfaces are the new Command Line
---


A lot of noise has been made of late re: chat interfaces and chat bots. People seem to think that they are new, revolutionary, and about to disrupt everything. No seriously, a lot of noise. Just look:

* [https://medium.com/point-nine-news/are-chat-bots-a-feature-or-a-product-ce3aa3e8506a#.knia925kf](https://medium.com/point-nine-news/are-chat-bots-a-feature-or-a-product-ce3aa3e8506a#.knia925kf)
* [https://medium.com/@Borthwick/introducing-botwick-want-a-bot-got-a-bot-botwick-and-how-to-roll-your-own-a4253512c652#.sw5e60rl0](https://medium.com/@Borthwick/introducing-botwick-want-a-bot-got-a-bot-botwick-and-how-to-roll-your-own-a4253512c652#.sw5e60rl0)
* [https://medium.com/@rob_ellis/slack-superscript-rise-of-the-bots-bba8506a043c#.snhn9e3k1](https://medium.com/@rob_ellis/slack-superscript-rise-of-the-bots-bba8506a043c#.snhn9e3k1)
* [https://medium.com/stephen-keep/app-fatigue-chatbots-maybe-the-answer-d976253193c0#.s5f9hnu82](https://medium.com/stephen-keep/app-fatigue-chatbots-maybe-the-answer-d976253193c0#.s5f9hnu82)

Which, honestly, has led me to a resounding "duh!"

Of course there are many tasks for which smartphone apps suck. Of course there are plenty of cases in which a power user might want to access a service at a lower level. Essentially, Of course the Command Line is still relevant.

This new found focus on chat bots and chat interfaces is nothing new. It's just the latest packaging that we're wrapping around the command line. Please allow me to explain:

The dawn of home computing really started with the birth of the command prompt. Suddenly, it was possible to type a sequence in to a computer and recieve a result. As a user of a modern computer, this hardly seems worth mentioning but, at the time, it was literally game changing.

For the next 20 years (or longer, depending on which industry you ask), the command line was the dominant way to interact with a computer. Early versions of Windows were just applications that ran on top of a command line interface, and they were pretty clumsy. If you wanted to get serious work done, you used the command line. Even today, many web development tasks are still accomplished most readily from a Linux shell. For most nerds, this is both obvious and unimportant. For everyone else, yes, we really do work like that.

![][2]

But, and this is the surprising bit for most non-technical users, in a lot of cases it really is preferable to work from a command line. On a PC it's faster to type out a short string than to move the mouse through a series of menus, in the same way that it's faster to slap ctrl-Z than it is to find the Undo button. Provided that you can remember the syntax and the commands necessary to cause the desired effects, which is really the crux of the command line problem.

Computers are dumb. They do exactly what they are told, and rarely anything else. It's easy to make yourself misunderstood, and frequently difficult to convey just the right message. This is a problem that has been studied at length for many years. Some software developers have built really swell natural language processors (Way back when, there was Infocom. Later, Apple's Siri, and Microsoft's Cortana come to mind), but anyone who has used one of these at length knows that they still leave a lot to be desired.

Of course the rise of cloud computing in the browser means that everyone (well, almost everyone), now conducts the majority of their day through (ever changing, instantly updated) browser based GUIs. It would be easy to claim that the command line was dead, but that's simply un-true. The command line has just been bolted on to the SMS, Chat, and Messaging apps we already use.

Thanks to advances in natural language processing, and the fact that individual bots only handle a relatively small number of operations, bots are on the rise. This is great for users and developers.

For users:

* Faster than a dedicated app for many tasks
* No apps to install means less storage space used, and no mucking about with the app store
* You're already using Messenger, iMessage, or Hangouts all the time.

For developers:

* No one has to approve your chat bot before users can connect with it
* No fancy-schmancy UI to design and implement
* Can be built in simple tools (Python, Perl) and run on a server you control

Granted, everything isn't sunshine and daisies:

* Facebook Messenger, for example, has a bot SDK but is only allowing a small number of developers to access it at this time.
* SMS bots are more expensive than bots that communicate over XMPP or another internet based messaging service, because you have to pay for each message sent.
* Folks in the US still aren't terribly used to interacting with web services in this way, so it might take a while for the trend to catch on like it has in China or India.
* Chat bots can't interact with local files. Depending on the chat platform, they may or may not be location aware, or capable of payment processing.
* Language processing is still in it's infancy

But even with those hurdles to adoption, I think it's worthwhile for many web developers to start focusing their attention on implementing proof-of-concept and Minimum Viable Products as chat bots. We're only going to see more of them in the future.

[1]: https://cdn-images-1.medium.com/max/600/1*RUD6vylzeUaN3Kz0EV1e0g.jpeg
[2]: https://cdn-images-1.medium.com/max/2000/1*AeFmAZTEGrX_nTCpUdKJqQ.jpeg
