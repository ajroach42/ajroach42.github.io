---
layout: post
category: post
published: false
title: A Modern Office with Vintage hardware
---
I've been toying iwth the idea of a building a modern office around 8 and 16 bit microcomputers from the 1980s and early 90s. This is an idea that I dig up every few months and play with for a few hours before discarding it because it's impractical and expensive. This is a description of my current version of this idea, and how it would work in practice. 

**DISCLAIMER** *Please understand, I recognize that implementing this would be both impractical and expensive, and that the same goals can more readilly be accomplished by myriad other methods. I know this, and yet I still can't abandon this hypothetical future. Don't consider this a blueprint, or if you do consider this a blueprint, don't hold me responsible if it is less fun and more tedious in practice than it sounds in theory. I'm probably going to do most of these things over the coming months, and I'll document as much as I can, eventually on it's own project page.*

If we're going to use a bunch of dinosaur computers to power a modern home and office, it's important for us to define the kind of work that will be done in that home/office, and for us to get specific about the dinosaurs. I am envisioning my own workplace, as I would prefer it to be, so I am focusing on the kinds of work that I do. At the end, I'll do a short piece of design fiction describing this office, and the work they do from the perspective of a prospective client. Maybe one day I can make this a reality. 

# Work 

So, my average day consists of the following activities: 

- Writing: I write a lot. Many thousand words a day across various platforms. 
- Email: So much of what I do on a day to day basis, both personally and professionally, is still handled through email. Much of the writing I do has an Email as it's final destination. 
- Live Chat: I interact with my co-workers and colaborators via chat. Mostly, this takes the form of Skype for Business or Microsoft Teams or Slack or Rocket.Chat or Jabber or... well, you get the idea. 
- Research: I spend a large portion of my day researching, both professionally and personally. I do a lot of this research via the web, and some of it via gopher. 
- Graphic Design: Well, really, graphic design adjacent. I do basic image editing, I do layouts for print projects. I do web design. 
- Publishing: I publish web pages, blog posts, and other content online. I also publish print versions of some of the designs mentioned above.
- Development: I write web applications, Linux CLI application, and Desktop and Mobile apps for multiple platforms. 
- Data entry: I don't do this as much anymore, but there was a time when a lot of my day was spent logging information in to databases and running reports. Traditionally, I have done this either through a web application (that I wrote) or a desktop/CLI application (that I wrote.)
- Calendar: I, unfortunately, need to hop in and out of meetings and phone calls throughout the day. A calendar application with notifications (and and some kind of public interface with outlook or gcal for scheduling) is essential. 

Beyond that, a portion of my job is and will continue to be troubleshooting client environments. That means I need to be able to manage VPN connections, and SSH/RDP/VNC sessions as appropriate. 

The above covers a surprisingly large portion of the work I do both professionally and personally, and the work I want to continue to do in the future. But computers are no longer (and have never really been) solely a tool for work. If you include my smartphones and streamaing devices, I am using a computer for 80% or more of the time that I am awake. 

Outside of the work I do, I also listen to a lot of music, both via my computer and from other sources, I spend most of my day with Mastodon up on some device or other, I read books, I watch movies, I listen to podcasts, I administer servers, I manage a todo list, I play games, I write games, I have been known to make music, edit podcasts, and even make the occasional video. 

# Hardware 

I'm fairly confident that every activity I've outlined above can be done to a greater or lesser extent by making use of various piece of vintage hardware. 

First, let's define which hardware I want to use: 

- Apple IIc
- Tandy 102 or Olivetti m10 
- Mac Classic II or Mac SE/30 
- HP 200 LX 
- Psion Series 5
- Atari ST BOOK or Atari STacy or Atari ST 
- eMac (1.42 GHz PowerPC G4 circa 2005) or g3 clamshell iBook or g4/g5/early intel iMac 
- Some dumb terminals (vt100, etc.)
- Phones! (Any of the various brightly colored vintage phones of the 50s, 60s, and 70s.)
- TVs and Monitors (specifically, a Philco Predicta, Panasonic/National Flying Saucer, Keracolor Sphere, JVC Video Sphere, and other interesting Space Age TVs)

I'll supplement the above with a small collection of raspberry pi's or other cheap machines running older OSs or emulating older machines, as well as acting as file servers, application servers, and gateways for the vintage machines.

Every machine on that list has been selected for a few reasons: 

1) Most of the items on it are portables, compact units, or otherwise power effecient machines. 
2) Nearly all of them have a very striking visual design that makes them look somehow both ancient and futuristic (that is to say, they tend to look like something out of Yesterday's Tomorrow, rather than today's.) 
3) They can be augmented by the addition of the best modern hardware. For most of them, this means Wireless networking, solid state storage (via CF or SD cards), and low power displays. 

These machines are from various eras, and out of the box they are all but entirely incompatible with each other and the modern world. Well, that last bit isn't entirely true. Nearly all of these computers can be made to understand one another via plaintext and serial-port networking in much the same way as they were able to interact with one another durring the BBS era. This will be important. 

## Supplemental Hardware

A large portion of the magic that enables us to use vintage computers (and other hardware) in a modern context is going to come down to the supplemental hardware. A lot of this ends up being custom, and vendors pop up and disappear all the time, so I'm not going to discuss individual products as much as classes of product. 

**Video Adapters**

**SD Card floppy drives** 

**SCSI to CF or SD adapters** 

**Serial-to-Bluetooth adapters** 

**Serial-to-Wifi modems** 



## Apple IIc 

### Why? 

It was seeing an Apple IIc in person for the first time recently that started me down this path again. The IIc is not a particularly important or impressive computer in terms of performance. It's essentially just an Apple IIe in a smaller case, and with some intigrated periphrials. For me, what makes it stand out are two key features: 

1) It's pretty dern power effecient, drawing 18 watts on average (without a screen.) While that's more than, say, a Raspberry Pi, it's so much less than a) most other vintage computers, b) most modern computers. 

2) It was produced right in the moment when Apple decided to embrace svelte industrial design for the first time (a trend they would return to again and again.) It is a small and unassuming package, and clearly a product of the 1980s (19a0s?), but it has an *almost* timeless look to it, as well. 

Beyond that, it has a few more things going for it. Namely, it has a standard serial port built in (more on this later), it has composite video out (for connecting to those TVs!) and modern hardware readilly available to give it access to [Solid State Storage](https://www.bigmessowires.com/shop/product/floppy-emu-model-b/) and [modern monitors](http://www.a2heaven.com/webshop/index.php?rt=product/product&product_id=135). It loads to applesoft BASIC which is widely documented and easy to use, and has multiple (good/interesting) graphics modes. 


### How? 

The Apple IIc could be used in the following fashions: 

- As a terminal connected to a modern linux machine either via a null modem cable or a serial-to-bluetooth or serial-to-wifi adapter. We'll discuss these hardware options, and the software that would run on the server, in more detail later. Importantly, a wifi connection would enable multiple machines to share a single modern computer as an application server. Dozens, if not hundred, of concurrent users could get by on a single Raspberry Pi. (https://github.com/dschmenk/apple2pi)

- The same null modem/wireless serial setup can be combined with vintage programs from the Apple II library or newly written/custom software for the Apple II to enable it to serve as a Word Proccessor, Gopher/Web browser/server, BBS browser/server, or other custom applications.

- Specifially, I could see the IIc serving as the interface to a Point of Sale system or the front-end for a custom database driven application. It's variety of hardware I/O, and the low level access to the hardware available from the machine combine to also make it an attractive choice for home automation tasks, or other projects that require directly interfacing with external hardware (much like a modern microcontroller, but arguably more capable and certainly easier to interact with) .  

- A game console (with a HUGE library of games https://archive.org/details/apple_ii_library_4am)

- 

## Tandy 102 // Olivetti m10 

## Mac Classic II or Mac SE/30

## HP 200 LX

## Psion Series 5 

## Atari 

## Emac 

## Dumb Terminals 

## Phones

## TVs and Monitors 

## Newer Machines 

# Other potential machines

## Armiga 

## Cambridge Z88

## Risc OS on Pi 

## 