---
layout: post
category: post
published: false
title: A Modern Office with Vintage hardware
---
I've been toying with the idea of a building a modern office around 8 and 16 bit microcomputers from the 1980s and early 90s. This is an idea that I dig up every few months and play with for a few hours before discarding it because it's impractical and expensive. This is a description of my current version of this idea, and how it would work in practice. 

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

## Serial Terminals 

### What?
This is a quick rundown of the software that we would run on a modern machine that older machines would interface with while acting as a serial terminal. This could also be done with a traditional serial terminal like the one pictured here. The point of this section is mostly to demonstrate how much of your day-to-day activities can be acomplished from a unix commandline. 


### Why? 

It may seem silly to simply use an old computer to connect to another computer and run applications on that other computer, but I think that many of the computers on this list have enough going for them on their own (long battery life, sunlight readable screens, interesting formfactors, surprising speed) to merit using them in just that fashion. Plus, the needs of a large number of vintage computers can be met by a single terminal server, and wireless adapters exist. 

If you're unfamiliar, the Unix/Linux command line is a surprisingly robust platform, that is very tollerant of being accessed in a variety of unusual ways. It takes some configuring and there is a learning curve, but once you're comfortable, you can get an astounding amount of work done. 

### How? 

Lets revist my original list of tasks, and break each one of them out over a serial terminal. Keep in mind that every machine on this list will have access to these applications over a wireless connection, so later when we are rating the various merits of the individual machines, we will lump their ability to do all of these tasks via Serial connection in to a single score. 

Writing:

Email: 

Live Chat: 

Research: 

Graphic Design: 

Publishing: 

Development: 

Data entry: 

Calendar: 

Music:

Mastodon:

books:

movies: 

podcasts: 

SSH/RDP/VNC:

todo list:

games (playing):

Games (writing): 

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

**Serial Terminal** Use the Apple IIc as a terminal connected to a modern linux machine either via a null modem cable or a serial-to-bluetooth or serial-to-wifi adapter. The Apple IIc can display 80 collumns of text, which makes it an ideal candidate for serving as a [Thin Client](https://en.wikipedia.org/wiki/Thin_client) in this fashion. 

We'll discuss the software that would run on the server in more detail later 

Importantly, a wifi connection would enable multiple machines to share a single modern computer as an application server. Dozens, if not hundred, of concurrent users could get by on a single Raspberry Pi. 

**As a Stand alone computer** The same null modem/wireless serial setup can be combined with vintage programs from the Apple II library or newly written/custom software for the Apple II to enable it to serve as a Word Proccessor, Gopher/Web browser/server, BBS browser/server, or other custom applications, while still interfacing with a modern networked world, complete with version control. 

The Apple IIc (and later the IIc Plus) is a fast machine, compared to many of it's contemporaries. It has a lot of RAM compared to it's contemporaries, and it can be put in to service as an excellent addition to your digital arsenal. 

Specifially, I could see the IIc serving as the interface to a Point of Sale system or the front-end for a custom database driven application. Its variety of hardware I/O, and the low level access to the hardware available from the machine combine to also make it an attractive choice for home automation tasks, or other projects that require directly interfacing with external hardware (much like a modern microcontroller, but arguably more capable and certainly easier to interact with). 

And I know the BBS line sound like a throwaway comment. It's not. I don't think we'll get to it in this post, but BBS connections can be a lot of fun, and super useful, if handled correctly. 

**A game console** There is a [HUGE library of games available for the Apple II](https://archive.org/details/apple_ii_library_4am), and the IIc is compatible with very nearly all of them. It might not be the most professional choice in the world, but the Apple IIc is hard to beat as a retro game console. 

**Development Environment** The Apple II line runs Applesoft BASIC which is a derivative of Microsoft BASIC which became QuickBASIC and GW-BASIC and BASICA and... well, basically programs that will run in BASIC on the Apple II can either run or be ported to run on many computers without a lot of fuss. Additionally there are Apple II emulators for dozens of computers, and even one that will [run in modern web browsers](https://www.scullinsteel.com/apple2/#hhgttg). 

![screenshot (4).jpeg]({{site.baseurl}}/images/screenshot (4).jpeg)

To me, that makes the Apple II an attractive choice as a development platform, with a set of strengths and quirks that keep it interesting and fulfilling. 



### Scorecard

**Writing:**  4/5
Good keyboard. Can write directly on the machine and transfer files via flash media or wirelessly. 

**Email:** 2/5
BBS based email only 

**Live Chat:** 2/5
BBS based chat only 

**Research:** 2/5 
Can access BBSs directly. May be able to run a Gopher browser. 

**Graphic Design:** 1/5 
Several vintage graphics packages are available, but a lack of support for modern file formats, and the low resolution of the screen render this machine an unlikely choice for design work. 

**Publishing:** 0/5
I'm not aware of any viable page layout software for print publishing, nor of drivers for modern printers. 

**Development:** 3/5
No IDEs, but a good built in language and few bugs or physical constraints. 

**Data entry:** 4/5
Good built in programming language, wireless networking, and a high resolution screen mean that this is a perfect target for data entry. 

**Calendar:** 0/5
No real time clock = no calendar. 

**Music:** 0/5
Only chiptunes. 

**Mastodon:** 1/5
No native Mastodon app available (but it would be possible to build one)

**Books:** 0/5
While it might be possible to rig up an ebook reader, why would you? 

**Movies:** 0/5
No video playback.

**Podcasts:** 0/5
No audio support.

**todo list:** 3/5
It would be possible to cobble together a decent to-do list manager in BASIC, that syncs back to our central file server, but it would probably be better to do this through your application server. 

**Games (playing):** 5/5
Huge library of great games.

Games (writing): 3/5
Is a great platform for playing games, but it does not provide many tools for creating them. That being said, Applesoft BASIC is a decent, reasonably fast platform, and does not feel limiting. 

Serial Terminal: 5/5
Wireless, no adapters, fast, high resolution. Hard to beat. 


## Tandy 102 // Olivetti m10 

### What?

![15635.jpg]({{site.baseurl}}/images/15635.jpg)

The first truely portable computer! Released under a dozen different names, with stylistic changes between each model, this cutie will run for weeks (months?) on a set of AA batteries. It's got a built in serial port, a good keyboard, and a screen that's just big enough to get stuff done. 

### Why? 

I used a Tandy 102 for several hours a day for about two years. It's a Great computer, and I'd still be using mine if it hadn't developed some display issues. It is small enough and light enough and sturdy enough to toss in a bag and take with you on the road. The memory is large enough to hold a few dozen pages at a time. It's easy to interact with modern computers (provided you have the right cables) and it'll last for around a month of daily use on a set of rechargable AAs. 

It's very nearly the perfect laptop. Plus the Olivetti version is one of the cutest computers I've seen in my whole life. 

It's also popular in the HAM radio community for doing SDR and packetBBSs, I've heard. 


### How? 

The TRS-80 Model 100/Tandy 102/Olivetti m10 is useful to a modern office in exactly two ways: 

- As a wireless serial terminal (over BT or wifi, doesn't matter.) The Tandy's screen displays just barely enough text to do useful things. 

- As a distraction free portable word proccessor (although even this is easier and more fun if you're just using it as a serial terminal to a linix box running your favorite text editor.) 

Having used this one pretty extensively, I feel comfortable saying that you should *not* try to use these computers as stand alone machines. They don't have the horsepower. They don't have the RAM. They were never designed to live on their own. 

But, as a wireless terminal connecting back to a raspberry pi (or an android phone! or a remote server) it can really feel magical. The screen has decent contrast. You can mostly read it in the sun. I've used mine for email, chat, and some basic web/gopher browsing. I've written blog posts on it, and published websites. I've played Zork. Heck, I've solved serious production issues on client servers from the park, with the Tandy connected to my phone's hotspot over wifi, and my phone providing a VPN connection through which I could telnet to my server, and SSH from my server to the client environment. 

It is a full fledged computer. You can do spreadsheets or write your own programs directly on the device. Some people really get a kick out of that. I never did, but I'm grateful for the ways that they continue to extend it. 

## Mac Classic II or Mac SE/30

### What?
![Se30.jpg]({{site.baseurl}}/images/Se30.jpg)

When you think about the Classic Mac, you probably think about something that looks like the Classic II or the SE/30. They are similar enough in all the important respects that I really don't differentiate between them. 

They have 9" monochrome screens, ~2MB of RAM, and an internal hard drive. The SE/30 can support up to 128MB of RAM while the Classic II tops out at 10MB. They both consume about 70 Watts in use.  

### Why? 

Cause they are heckin' cute! But also for more reasons! They were released circa 1989, and supported up through the early 00s, which means that there is a TON of software written for these things out on the market, including office suites, web browsers, gopher browsers, desktop publishing platforms and all manner of other things. 

They have built in HDDs, which use SCSI. That means we can swap in SD cards in place of the HDDs. They are small, and light. They are easy to crack open and work on, and they are reasonably modern (compared to the other computers we've discussed so far.) 

They have RS-422 serial ports instead of the more common RS-232, but these are directly compatible and adapters aren't hard to find. 

What really makes the classic macs magic, for me, is the software. Mac OS System 7 is honestly great, and they can run [Hypercard](https://blog.archive.org/2017/08/11/hypercard-on-the-archive-celebrating-30-years-of-hypercard/). Hypercard deserves (and will eventually get) a post of it's own, but it's essentially the fastest and easiest way for non-technical users to create applications. 

Think Powerpoint + some of the least bad features of the internet + a really simple and easy to understand method of responding to user inputs and you'll land somewhere in the neighborhood. Hypercard is worth the price of admission. I want to keep a compact macintosh in my home specifically for exploring hypercard.  



### How? 

**Hypercard** First and foremost, Hypercard is the best. As a rapid application prototyping tool, or even as a final destination for your application. It's a pain to get hypercard stacks running on modern computers, but if you're building internal applications I can't think of a better platform to do it on. 

**Serial Terminal** Just like everything else, Compact Macs make excellent candidates for serial terminals. In this case, though, the Mac can actually multitask. That means that you can check your email in a terminal connection while also working on your hypercard app. 


**Standalone computer** There are email clients, office programs, web browsers, FTP apps, and all manner of other goodies that will run happily on system 7.5 with 2MB of RAM. Most modern computer tasks can be done on this computer. Toss in an adapter and a wireless modem and you have a really interesting little box. 


## HP 200 LX

### What?

![Hp200lx,_open.jpg]({{site.baseurl}}/images/Hp200lx,_open.jpg)

My favorite computer on this list, the HP 200LX is a weird little relic. It was originally released in 1994, and is the third in a line of **palmtop** computer released by HP in the early 90s. It's an IBM PC Compatible DOS computer, built around a 186 proccessor with a greyscale CGA compatible screen and a whopping 2MB of RAM, it will run for weeks on 2 AA batteries. (No really, I've done it.) 

### Why? 

Again, because it's heckin' awesome. It's got a sunlight readable screen, the largest software library of any computer we've discussed so far, built in support for PCMCIA storage devices (and therefore CF cards.) It runs DOS, which is my favorite OS of the 1980s, if only because it's the one I've had the most direct experience with. 

Also, it has a great callendar app, a good set of programs to sync with (more) modern computers, and a tiny RS-232 compatible serial port. 

### How? 

**ebook reader** it's a sunlight readable, handheld clamshell device that'll run forever on a pair of rechargable AAs. Couple it with Vertical Reader (or VertReader or VR) by Giles Kohl and you've got yourself the best little ebook reader. I used mine to read A Princess of Mars at the beach in 2007. 

**Standalone** It's a palmtop computer! With a CF card slot that you can use to transfer files to from another computer. There are hundreds of applications written specifically for this machine, and it is compatible with (tens of) thousands of DOS applications. Add an RS-232 Wifi modem and It'll run SSH (slowly, but it'll do it) and a web browser (ARACHNE) and a gopher browser and all kinds of other neat stuff. 

It'll play Zork, it'll manage your email. It'll run Windows 3.1 or GEM or ... Look, I'll do an article about DOS in general and the HP LX line specifically in a few weeks. As a standalone computer, it's surprisingly powerful and fun. 

**Serial Terminal** Yep! This one can be a wireless serial terminal too. You gotta do some fancy stuff to get a wireless adapter to plug directly in without an additional cable, but it'll work. The keyboard is a little tight, and the addition of the numberpad was a Big Mistake IMO, but it's still a functional little machine to use while you're kickin' it on the couch. 

**Dev Environment** It runs DOS. You know what else runs DOS? Everything, thanks to DOSBox. It also has compilers available for dozens of languages, and my favorite text editor (edit.exe).

**PDA** I know that PDAs are passe in the era of the smartphone but hear me out. They are wonderful. Managing your callendar, your to-do list, and your contacts from a device that is also a full fledged computer and isn't pretending to be a phone is pretty wonderful. Using the same device to manage email, social media, and chat can also be pretty great. About the only things it won't do are take calls and media (which, incedentally, are things my phone is great at.)

## Atari 

### What? The Atari STacy and ST BOOK are laptops from the late 80s and early 90s. Both of them had greyscale screens. They are both members of the Atari ST family, which was Atari's entry in to the 16 bit home computer market.

The ST family ran Atari TOS under the hood, meaning a GUI and file manager (called GEM) that looks a lot like a classic mac. It could read and write from DOS compatible floppy disks. They have a large library of software, though not as large as the Mac or DOS library, and a surprisingly strong collection of real time music making applications. 

### Why? 

The ST BOOK is the computer from this line that I'd be most interested in incorporating in to our office. The ST BOOK was pretty lightweight, could run on AAs, and had surprisingly good battery life (it draws about 20 watts of power when in use.) It has a sunlight readable, non-backlit screen, no internal floppy drive (I consider that a plus!), and an intersting physical profile. Additionally, it had a pretty great set of interfaces: 

- MIDI x 2
- Serial Port x 1
- Paralell port x 1
- FDD/ACSI x 1 (can be converted to SCSI with a simple adapter)

All of that was rounded out with an internal HDD, mounted with a standard 2.5" IDE cable. That means that we can buy off the shelf IDE->CF or IDE->SD adapters to replace the moving hard drive with a solid state disk, resulting in a laptop with even better battery life, larger storage, and no internal moving parts. 

Various European vendors also sell add ons that can add USB mass storage, CF cards, or SD cards through the FDD/ACSI port found on most ST computers. Since TOS used an MSDOS compatible disk format, that means that you can swap these external storage disks with any modern computer, as well as any vintage DOS or Windows computer (with the appropriate adapters.)

### How? 

We've covered most of these Hows before. There is very little the ST line can do that is unique to the ST line beyond a couple of pieces of exclusive software. The ST line in general would excel in all the same places that a DOS machine or a compact Macintosh would excel (minus multi-tasking and hypercard, of course.) The ST Book would come with the advantage of a small, light formfactor and true wireless operation. Where this platform stands out, is in music production with lots of synth and tracker software and 2 MIDI ports, even on the ST BOOK, the ST line is right at home in a studio. 

If you're not making music, the ST can still hold it's own as a standalone machine, and as a serial terminal to a more modern machine. It can access BBSs and Gopher servers and handle email and basic web browsing. Plus, it has a nice keyboard and it looks neat. 

## G4 eMac, G3 iBook, G5 iMac 

### What?
Apple Macs from the early 00s. The newest machines on this list. I'm grouping them together because for practical purposes they are very similar. I will take a moment to describe their few differences: 

**G4 eMac** this was an iMac made for the educational market, and built around a CRT. It's big and bulbous and looks for all the world like a product of Braun circa 1965. It has a 16" screen running at 1280 x 960, and can support up to 1GB of ram. It has built in wifi, speakers, a DVD/CD combo drive, and can support up to Mac OS 10.5 

It's a heavy monster, and were it not for the fact that it's design fits my desired aesthetic so well, I wouldn't be considering it. It's also a surprisingly powerful and capable machine. 

**iBook G3** slightly older than the eMac, this is a laptop originally launched in 1999. Known for it's candyshell design, the iBook G3 feels less like a modern machine in use than either the emac or the G5 iMac. The system is equipped with an 800x600 display, and shipped with 64MB of RAM (expandable up to 512MB.) It originally ran Mac OS 9, but can be upgraded up to 10.3. It features USB 1.1 ports, firewire, and wifi. 

Compared to the eMac or the G5, the iBook begins to look and feel like a toy. It isn't, and it has a few tricks up it's sleeve that we'll discuss in a moment. 

**iMac G5** It almost feels like cheating to put the G5 on this list. Almost. But the things that make the g3 and the g4 attractive to me for this purpose apply just as much to the g5, while also giving us the benefit of a much more powerful computer. 

When you think white plastic iMac, you think of the g5. With a 20", 1680 × 1050 display, a 2.1 GHz powerPC proccessor, up to 2GB of RAM, and up to 500GB HDD, the G5 iMac is very nearly a modern computer. If it had an intel chip inside (like the model that replaced it), it likely would have continued to recieve updates trough 2011 or later. As is, though, it got left in the dust by the shifting tides of corporate favor. 

For us, that's great news. It's a beautiful machine, with more juice than 10 of pretty much anything else on this list. It runs a decidedly modern operating system, and has access to a large software library. 
 

### Why? 

The Why for this one is almost too easy. All PowerPC macs can run classic Mac software. That means that every computer in this group has access to Hypercard. Plus, intrepid hackers are still out there building modern software for OS X 10.5 and some even build for Mac OS 9.x. Plus each of them has a decidedly unique and nearly iconic look. 


### How? 
Every computer in this group can be used in most of the same ways you would use a brand new computer (although you may ocassionally get frustrated using the iBook in this fashion) while also providing access to a wealth of vintage software and the best non-technical application development platform ever made. 

Beyond that, Mac OS 9 (available on the iBook) uses a Cooperative Multitasking model. That means that it's effectively single tasking, relying on the foreground application to pass control to other applications. For a lot of things, this is pretty shitty, but it means that the running application gets unprecendent access to system resources. That means that tasks which seem to creak under OS X on the iBook or eMac will feel Much more responsive under OS 9. 

The eMac G4 or the iMac G5 would make a great media player, audio editor, graphics editor, or even video editor. They have modern web browsers, and support modern encryption protocols. I learned graphic design, audio engineering, and video editing on an eMac. 

The iBook would make a solid audio workstation under OS 9. It would make a usable, if slow, immitation of a modern computer under OS X. Under either OS, we could treat the iBook like one of our older machines. Using it as a serial terminal, focusing on it's strengths (hypercard, audio editing) and offloading more proccessor intensive tasks to a newer machine. 

Uisng the iBook with OS X we could run locally many of the same applications that we would access remotely from a serial terminal. That is to say that OS X gives us direct access to a Unix command line, which would enable us to access BBSs, email, web browsers, and a whole mess of other command line applications, without having to rely on a mainframe. 

Plus, you know, there's Hypercard. 





## Phones

### What?

### Why? 

### How? 

## TVs and Monitors 

### What?

### Why? 

### How? 

## Newer Machines 

### What?

### Why? 

### How? 

# Other potential machines

## Armiga 

## Cambridge Z88

## Risc OS on Pi 

## Psion Series 5 
