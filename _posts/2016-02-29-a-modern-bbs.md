---
layout: post
category: post
splash-wide: /images/DEC_VT100_terminal.jpg
tags:
  - 'null'
published: true
title: 'A Modern BBS: Reviving the local, distributed, weird precursor to Facebook.'
---
[BBSs][7] were a weird, wonderful facet of early computer culture, connecting community members in to a distributed, often free, local social network. I want to revive this almost forgotten concept, and find a modern spiritual successor.

![][8]

Photo by [Jason Scott][9]

#### History Lesson

Way before facebook, before the web in general, if you wanted to argue with strangers about politics you connected to one of your local BBSs. These were kind of like small, private, local, social networks. The BBS was just a computer in someone's home, and you connected to it by calling it from your computer. Dozens of people from your region (long distance was expensive) might also connect to this same BBS, and it was used by and large the way one might use facebook today.

The important things to remember about these early BBSs:

— They existed separate from the modern internet.

— You connected directly to the BBS, by calling its phone number, rather than connecting to a single network that had access to many different pages.

— Anyone with a computer and a modem could run a BBS. There were no gatekeepers.

— Anyone with a computer and a modem could connect to a BBS, as long as they could afford the phone bill.

![][10]

Many early BBSs were run on C-64s

Imagine it, a private/local anonymous/pseudonymous social network that required no additional infrastructure beyond that which has existing since Alexander Graham Bell invented telephony. A private, local, distributed, weird internet, complete with email ( [even cross-system email][11] ), [online games][12], public messaging, and [a culture][13] all it's own.

![][14]

We're going to need something more advanced than this, for the modern age.

As the internet matured, BBSs died away, and that's a real shame, because BBSs were an astounding, and important development in early computing history and culture that has been all but lost today. I want to see this concept brought to modern technology to build a new, distributed, local, social network free from the privileges and restrictions of the internet, and I think it can be done in a new, and intentionally radical way.

#### Reviving the BBS

It is possible to build a BBS style system today using small, cheap, modern technologies and free software. One such project, [PirateBox][15] (or the more ethically names [Library Box][16]), can be run on the ridiculously cheap [Raspberry Pi 0][17], (When coupled with the necessary power supply and USB adapter.) Setup isn't incredibly straightforward, since the Pi 0 doesn't have an ethernet port, but it can be done with only minor frustration (I'm sure I'll write about it at some point.) Once configured, you'll have a bulletin board, a chat room, the ability to upload files, and a UPnP streaming server. It may not sound like much, but it can be revolutionary on a college campus, or in an apartment building.

![][18]

The Library Box, one of many modern BBS like systems

There are other projects in the works (including one of my own) that aim to cover some of the same ground, that is, that aim to use cheap and readily accessible computers as a convenient way to serve up information, media, and communication tools for anyone in physical proximity. Of course, the biggest limitations of a system like this are:

* The Wifi signal has a relatively limited range, meaning you can only access this system when you're in the same (or possibly an adjacent) building.
* There isn't, at the moment, a reliable way to pass data between these islands

Even with these limitations, a community can build quickly around a well placed modern BBS. For a few months last summer, we ran one at [Analog Revolution][19], and we watched it quickly become a place for community discussion, and the sharing of (among other things) local music. Eventually, the hardware was cannibalized for further experimentation, but as a dry run the Analog BBS affirmed my belief that this is a viable, necessary, and potentially vital next step in the evolution of modern computing.

#### Surmounting the Obstacles

Over the next several months, I'll be working to overcome some of the obstacles I mentioned above. (If you'd like to [follow my progress, sign up for my newsletter.][20], I'm sure this topic will feature heavily in rotation.) My plan at the moment is to build several of these BBS nodes, powered by the newly released [Raspberry Pi 3][21], and to deploy them in several strategic locations throughout my community.

![][23]

One potential solution for long range communication.

From there, I want to enable long range communication with these nodes. Ideally, using something akin to the [GoTenna][24] radios, but possibly using something like the [xBee][25]. This should enable client -> server connections over distances for 1–4 miles. In the long run, it is my hope to enable each of these nodes to connect together over a [mesh network][26], enabling access to a local, distributed, surveillance resistant, censor proof, and unabashedly bizarre replacement-internet.

#### Why bother?

Because we can! Because it's fun! Because it'd be really cool. But also, because our infrastructure is brittle, fragile, and haphazard. Because [governments can disable the internet][27] for their citizens. Because, when the NSA isn't spying on you, [Facebook is.][28]

![][29]

Who's with me?

We don't deserve any better, either. We've given these large, private corporations access to every aspect of our lives. We won't deserve better until we demand better, and create it for ourselves. We have the opportunity to take back our digital liberty, to connect with our local community, to fight the race towards homogenized culture, and to do something fun.



Of course, this might all be little more than a pipe dream but, the technology is there, the [need is there][30], and wouldn't it be something if we could pull it off?



[7]: https://en.wikipedia.org/wiki/Bulletin_board_system
[8]: https://cdn-images-1.medium.com/max/1600/0*EbptUQmjV24JW-_N.jpg
[9]: https://www.flickr.com/people/54568729@N00
[10]: https://cdn-images-1.medium.com/max/1600/1*3gNJEq62qKM2RszIRIFfUg.png
[11]: https://en.wikipedia.org/wiki/FidoNet
[12]: https://en.wikipedia.org/wiki/BBS_door
[13]: https://www.youtube.com/watch?v=JnSz-Hb9LQY
[14]: https://cdn-images-1.medium.com/max/1600/1*5fzHMD7KmWukT3aK5rDrJA.jpeg
[15]: https://piratebox.cc/
[16]: http://librarybox.us/
[17]: https://www.raspberrypi.org/blog/raspberry-pi-zero/
[18]: https://cdn-images-1.medium.com/max/1600/1*bTcVfIPGcx45Yu2DoRW5Uw.jpeg
[19]: http://analogrevolution.com
[20]: http://tinyletter.com/ajroach42
[21]: https://www.raspberrypi.org/blog/raspberry-pi-3-on-sale/
[23]: https://cdn-images-1.medium.com/max/1600/1*Iuikav1W5ma-4oM_d81j3A.jpeg
[24]: http://www.gotenna.com/
[25]: https://www.sparkfun.com/products/9099
[26]: https://en.wikipedia.org/wiki/Mesh_networking
[27]: http://www.wsj.com/articles/SB10001424052748703956604576110453371369740
[28]: http://www.businessinsider.com/this-is-how-facebook-is-tracking-your-internet-activity-2012-9
[29]: https://cdn-images-1.medium.com/max/1600/1*i5Ekawy3LGYLsT2Hr1NIvQ.jpeg
[30]: https://www.eff.org/nsa-spying
