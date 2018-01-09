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
- Literally any other neat computer I come across (like the Amiga Video Toaster) can and likely will be worked in to this blueprint over time. 

I'll supplement the above with a small collection of raspberry pi's or other cheap machines running older OSs or emulating older machines, as well as acting as file servers, application servers, and gateways for the vintage machines.

Every machine on that list has been selected for a few reasons: 

1) Most of the items on it are portables, compact units, or otherwise power effecient machines. 
2) Nearly all of them have a very striking visual design that makes them look somehow both ancient and futuristic (that is to say, they tend to look like something out of Yesterday's Tomorrow, rather than today's.) 
3) They can be augmented by the addition of the best modern hardware. For most of them, this means Wireless networking, solid state storage (via CF or SD cards), and low power displays. 

These machines are from various eras, and out of the box they are all but entirely incompatible with each other and the modern world. Well, that last bit isn't entirely true. Nearly all of these computers can be made to understand one another via plaintext and serial-port networking in much the same way as they were able to interact with one another durring the BBS era. This will be important. 

## Supplemental Hardware

A large portion of the magic that enables us to use vintage computers (and other hardware) in a modern context is going to come down to the supplemental hardware. A lot of this ends up being custom, and vendors pop up and disappear all the time, so I'm not going to discuss individual products as much as classes of product. 

**Video Adapters** The Apple II, Atari ST, and a bunch of other vintage computers that I have yet to research well enough to intigrate in to this plan (but I'll get there, promise) need an external monitor. Most of them have a low quality composite out, which will connect them to a TV, and a high quality output for connecting to a monitor. 

The high quality outputs, as a rule, do not use a standard VGA connector, but rather rely on video cables and video modes that no longer exist. As a result, if you want to use a vintage computer in the highest resolution and best quality available, you're stuck getting a vintage (power hungry!) monitor, or reaching for an adapter. 


**SD Card floppy drives** The Apple II, Mac Classic, Atari ST, the C64 and many other computers interacted with the world mostly via incompatible, fragile floppy disks. On most of these computers, the Floppy Disk drive can be replaced, or an external floppy disk drive can be attached. 

Various modern products exist that allow Floppy Disk *files* stored on SD cards to be loaded in to these computers as if they were actual disks. This is a great way to get programs and data in and out of vintage computers, and to keep them self contained (ie, not dependent on a modern computer.) 

**SCSI to CF or SD adapters**  SCSI was a hard drive standard used by late 80s and early 90s Macs like the Mac Classic II and the Mac Classic SE/30. It is possible to replace these (small/aging) hard drives with more modern solid state storage. 

This would be an Internal modification. The SD card is not removable, and is formatted by the computer directly. That means it looks and acts Exactly like a real hard drive. This is good for many reasons, but it does limit the viability of using this method to transfer files. 

**Compact Flash Cards** Compact Flash cards are neat! They are still widely available. Some computers (the psion series 5) used them directly for storage. They are pin compatible with the IDE standard used on most late 80s - late 90s PCs, requiring a simple pass-through adapter. 

They can also work with many laptops and portables (like the HP 200LX) via a Compact Flash to PCMCIA adapter. These are cheap ($10ish?). 

Regardless of how you connect your vintage computer to your PCMCIA card, you'll find that they are pretty easy to read on modern computers. Readers and adapters have been around for ages, and are cheap and abundant. 


**Serial-to-Bluetooth adapters** Did you know that bluetooth was designed to replace serial cables? Yep!  And the serial cable protocal is still baked into BT. There are a bunch of Serial -> BT adapters on the market. Many of them are built around the [RN-42](https://www.sparkfun.com/products/12574). 

Stick one of these on an 80s microcomputer (or a 90s palmtop) and you can interface wirelessly with another computer as if you were directly connected to it. This is perfect for terminals like the venerable vt100, but can also be used with any computer with a Terminal or Telnet program. 

**Serial-to-Wifi modems** Mostly, these are built around the [ESP8266](https://www.sparkfun.com/products/13678) which is widely available and dirt cheap. You can use a serial wifi modem to connect a vintage microcomputer directly to the internet, with no intermediary. You can also use it to provide remote access to computers on your network via telnet. 

[This product](http://biosrhythm.com/?page_id=1453) used to be the gold standard, but is no longer available. Others built around the same hardware will perform more or less identically. [Here's a blogpost about it](http://www.bytecellar.com/2017/05/30/the-wonderful-wifi232-bbsing-has-literally-never-been-easier/). 

And a video review:

<iframe width="560" height="315" src="https://www.youtube.com/embed/fsS0E4G310Y" frameborder="0" gesture="media" allow="encrypted-media" allowfullscreen></iframe>

The Wifi-232, or another ESP8266 based RS-232>wifi modem can make your vintage microcomputer a first class citizen on the internet. As far as your computer is concerned, it's just a modem. Furthermore, it can be coupled with some new custom code on several of these microcomputers to enable some *really* cool functionality. (More on this later.)  

**Analog to Digital Telephone Adapter** Because we want those groovy vintage handsets to be able to be used with VoiP calls. There are a bunch of different setups you can go for, but the most robust would almost certainly be running [Asterisk](https://en.wikipedia.org/wiki/Asterisk_(PBX)) along with a channel bank like the CISCO PAP2T. 

Another option would be to use an Obihai OBi110 or similar, which supports [SIP](https://en.wikipedia.org/wiki/Session_Initiation_Protocol) and [XMPP calls](https://en.wikipedia.org/wiki/XMPP) (and google voice, if that's your thing.) They aren't terribly expensive, and they interface with multiple free VoiP services, including some which can provide a bridge to POTS. 

For me, the primary use case for this setup would mostly be internal calls and one-on-ones, but the propspect of setting up a dedicated landline is pretty appealing. I might give this a shot soon, and report back with more detailed instructions. 

**TV Transmitter** This one might not be legal where you live, so be careful. You can mostly DIY it with instructions from [AntiqueRadio.org](https://antiqueradio.org/HomeTVTransmitter.htm)



## Apple IIc 

![By Bilby (Own work) [CC BY 3.0 (http://creativecommons.org/licenses/by/3.0)], via Wikimedia Commons]({{site.baseurl}}/images/1024px-Apple_IIc_with_monitor.jpg)
##### By Bilby (Own work) [CC BY 3.0 (http://creativecommons.org/licenses/by/3.0)], via Wikimedia Commons

### What? 

The Apple IIc was Apple's compact version of the Apple IIe. It's a small, self contained computer, with a fair amount of power and a great industrial design. 

### Why? 

It was seeing an Apple IIc in person for the first time recently that started me down this path again. The IIc is not a particularly important or impressive computer in terms of performance. It's essentially just an Apple IIe in a smaller case, and with some intigrated periphrials. For me, what makes it stand out are two key features: 

1) It's pretty dern power effecient, drawing 18 watts on average (without a screen.) While that's more than, say, a Raspberry Pi, it's so much less than a) most other vintage computers, b) most modern computers. 

2) It was produced right in the moment when Apple decided to embrace svelte industrial design for the first time (a trend they would return to again and again.) It is a small and unassuming package, and clearly a product of the 1980s (19a0s?), but it has an *almost* timeless look to it, as well. 

Beyond that, it has a few more things going for it. Namely, it has a standard serial port built in, it has composite video out (for connecting to those TVs!) and modern hardware readilly available to give it access to [Solid State Storage](https://www.bigmessowires.com/shop/product/floppy-emu-model-b/) and [modern monitors](http://www.a2heaven.com/webshop/index.php?rt=product/product&product_id=135). It loads to Applesoft BASIC which is widely documented and easy to use, and has multiple (good/interesting) graphics modes. It's FAST (for the time) and has a lot of RAM (for the time) and a huge software library (for any time.) 


### How? 

The Apple IIc could be used in the following fashions: 

**Serial Terminal** Use the Apple IIc as a terminal connected to a modern linux machine either via a null modem cable or a serial-to-bluetooth or serial-to-wifi adapter. The Apple IIc can display 80 collumns of text, which makes it an ideal candidate for serving as a [Thin Client](https://en.wikipedia.org/wiki/Thin_client) in this fashion. 

We'll discuss the software that would run on the server in more detail later 

Importantly, a wifi connection would enable multiple machines to share a single modern computer as an application server. Dozens, if not hundred, of concurrent users could get by on a single Raspberry Pi. 

**As a Stand alone computer** The same null modem/wireless serial setup can be combined with vintage programs from the Apple II library or newly written/custom software for the Apple II to enable it to serve as a Word Proccessor, Gopher/Web browser/server, BBS browser/server, or other custom applications, while still interfacing with a modern networked world, complete with version control. 

The Apple IIc (and later the IIc Plus) is a fast machine, compared to many of it's contemporaries. It has a lot of RAM compared to it's contemporaries, and it can be put in to service as an excellent addition to your digital arsenal. 

Specifially, I could see the IIc serving as the interface to a Point of Sale system or the front-end for a custom database driven application. It's variety of hardware I/O, and the low level access to the hardware available from the machine combine to also make it an attractive choice for home automation tasks, or other projects that require directly interfacing with external hardware (much like a modern microcontroller, but arguably more capable and certainly easier to interact with) .  

**A game console** There is a [HUGE library of games available for the Apple II](https://archive.org/details/apple_ii_library_4am), and the IIc is compatible with very nearly all of them. It might not be the most professional choice in the world, but the Apple IIc is hard to beat as a retro game console. 

**Development Environment** The Apple II line runs Applesoft BASIC which is a derivative of Microsoft BASIC which became QuickBASIC and GW-BASIC and BASICA and... well, basically programs that will run in BASIC on the Apple II can either run or be ported to run on many computers without a lot of fuss. Additionally there are Apple II emulators for dozens of computers, and even one that will [run in modern web browsers](https://www.scullinsteel.com/apple2/#hhgttg). 

![screenshot (4).jpeg]({{site.baseurl}}/images/screenshot (4).jpeg)

To me, that makes the Apple II an attractive choice as a development platform. 

## Tandy 102 // Olivetti m10 

### What?

### Why? 

### How? 



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