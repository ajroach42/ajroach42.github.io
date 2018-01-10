---
layout: post
category: post
published: true
title: A Modern Office with Vintage hardware
---
I've been toying with the idea of a building a modern office around 8 and 16 bit microcomputers from the 1980s and early 90s. This is an idea that I dig up every few months and play with for a few hours before discarding it because it's impractical and expensive. This is a description of my current version of this idea, and how it would work in practice. 

**DISCLAIMER** *Please understand, I recognize that implementing this would be both impractical and expensive, and that the same goals can more readily be accomplished by myriad other methods. I know this, and yet I still can't abandon this hypothetical future. Don't consider this a blueprint, or if you do consider this a blueprint, don't hold me responsible if it is less fun and more tedious in practice than it sounds in theory. I'm probably going to do most of these things over the coming months, and I'll document as much as I can, eventually on it's own project page.*

If we're going to use a bunch of dinosaur computers to power a modern home and office, it's important for us to define the kind of work that will be done in that home/office, and for us to get specific about the dinosaurs. I am envisioning my own workplace, as I would prefer it to be, so I am focusing on the kinds of work that I do. At the end, I'll do a short piece of design fiction describing this office, and the work they do from the perspective of a prospective client. Maybe one day I can make this a reality. 

# Work

So, my average day consists of the following activities: 

- Writing: I write a lot. Many thousand words a day across various platforms. 
- Email: So much of what I do on a day to day basis, both personally and professionally, is still handled through email. Much of the writing I do has an Email as it's final destination. 
- Live Chat: I interact with my co-workers and collaborators via chat. Mostly, this takes the form of Skype for Business or Microsoft Teams or Slack or Rocket.Chat or Jabber or... well, you get the idea. 
- Research: I spend a large portion of my day researching, both professionally and personally. I do a lot of this research via the web, and some of it via gopher. 
- Graphic Design: Well, really, graphic design adjacent. I do basic image editing, I do layouts for print projects. I do web design. 
- Publishing: I publish web pages, blog posts, and other content online. I also publish print versions of some of the designs mentioned above.
- Development: I write web applications, Linux CLI application, and Desktop and Mobile apps for multiple platforms. 
- Data entry: I don't do this as much anymore, but there was a time when a lot of my day was spent logging information in to databases and running reports. Traditionally, I have done this either through a web application (that I wrote) or a desktop/CLI application (that I wrote.)
- Calendar: I, unfortunately, need to hop in and out of meetings and phone calls throughout the day. A calendar application with notifications (and and some kind of public interface with outlook or gcal for scheduling) is essential. 

Beyond that, a portion of my job is and will continue to be troubleshooting client environments. That means I need to be able to manage VPN connections, and SSH/RDP/VNC sessions as appropriate. 

The above covers a surprisingly large portion of the work I do both professionally and personally, and the work I want to continue to do in the future. But computers are no longer (and have never really been) solely a tool for work. If you include my smartphones and streaming devices, I am using a computer for 80% or more of the time that I am awake. 

Outside of the work I do, I also listen to a lot of music, both via my computer and from other sources, I spend most of my day with Mastodon up on some device or other, I read books, I watch movies, I listen to podcasts, I administer servers, I manage a todo list, I play games, I write games, I have been known to make music, edit podcasts, and even make the occasional video. 

# Which Computers?

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

1) Most of the items on it are portables, compact units, or otherwise power efficient machines. 
2) Nearly all of them have a very striking visual design that makes them look somehow both ancient and futuristic (that is to say, they tend to look like something out of Yesterday's Tomorrow, rather than today's.) 
3) They can be augmented by the addition of the best modern hardware. For most of them, this means Wireless networking, solid state storage (via CF or SD cards), and low power displays. 

These machines are from various eras, and out of the box they are all but entirely incompatible with each other and the modern world. Well, that last bit isn't entirely true. Nearly all of these computers can be made to understand one another via plaintext and serial-port networking in much the same way as they were able to interact with one another during the BBS era. This will be important. 

# What else?

A large portion of the magic that enables us to use vintage computers (and other hardware) in a modern context is going to come down to the supplemental hardware. A lot of this ends up being custom, and vendors pop up and disappear all the time, so I'm not going to discuss individual products as much as classes of product. 

**Video Adapters** The Apple II, Atari ST, and a bunch of other vintage computers that I have yet to research well enough to integrate in to this plan (but I'll get there, promise) need an external monitor. Most of them have a low quality composite out, which will connect them to a TV, and a high quality output for connecting to a monitor. 

The high quality outputs, as a rule, do not use a standard VGA connector, but rather rely on video cables and video modes that no longer exist. As a result, if you want to use a vintage computer in the highest resolution and best quality available, you're stuck getting a vintage (power hungry!) monitor, or reaching for an adapter. 

**SD Card floppy drives** The Apple II, Mac Classic, Atari ST, the C64 and many other computers interacted with the world mostly via incompatible, fragile floppy disks. On most of these computers, the Floppy Disk drive can be replaced, or an external floppy disk drive can be attached. 

Various modern products exist that allow Floppy Disk *files* stored on SD cards to be loaded in to these computers as if they were actual disks. This is a great way to get programs and data in and out of vintage computers, and to keep them self contained (ie, not dependent on a modern computer.) 

**SCSI to CF or SD adapters**  SCSI was a hard drive standard used by late 80s and early 90s Macs like the Mac Classic II and the Mac Classic SE/30. It is possible to replace these (small/aging) hard drives with more modern solid state storage. 

This would be an Internal modification. The SD card is not removable, and is formatted by the computer directly. That means it looks and acts Exactly like a real hard drive. This is good for many reasons, but it does limit the viability of using this method to transfer files. 

**Compact Flash Cards** Compact Flash cards are neat! They are still widely available. Some computers (the psion series 5) used them directly for storage. They are pin compatible with the IDE standard used on most late 80s - late 90s PCs, requiring a simple pass-through adapter. 

They can also work with many laptops and portables (like the HP 200LX) via a Compact Flash to PCMCIA adapter. These are cheap ($10ish?). 

Regardless of how you connect your vintage computer to your PCMCIA card, you'll find that they are pretty easy to read on modern computers. Readers and adapters have been around for ages, and are cheap and abundant. 

**Serial-to-Bluetooth adapters** Did you know that bluetooth was designed to replace serial cables? Yep!  And the serial cable protocol is still baked into BT. There are a bunch of Serial -> BT adapters on the market. Many of them are built around the [RN-42](https://www.sparkfun.com/products/12574). 

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

# Serial Terminals

### What?

![vt100-1024x577.jpg]({{site.baseurl}}/images/vt100-1024x577.jpg)

Back in the day, before the era of the 8-bit Microcomputer, people didn't have computers. Organizations had computers. People had terminals that they used to connect to the computers owned by those organizations. Those connections could be over a local serial line (at a university or business) or over the phone. Importantly, these machines were shared, multi-user machines. Much of the way we interact with the web today is reminiscent of those mainframe days. 

This is a quick rundown of the software that we could run on a modern machine that could take input from these older machines and pipe output back to them. This could also be done with a traditional serial terminal like the one pictured here. Rather than interfacing through a serial cable, we expect these computers to interface with wifi or bluetooth modems. The point of this section is mostly to demonstrate how many of the activities I do on a regular basis can in face be done from the unix/linux commandline. 

### Why?

It may seem silly to simply use an old computer to connect to another computer and run applications on that other computer, but I think that many of the computers on this list have enough going for them on their own (long battery life, sunlight readable screens, interesting formfactors, surprising speed) to merit using them in just that fashion. Plus, the needs of a large number of vintage computers can be met by a single terminal server, and wireless adapters exist. 

If you're unfamiliar, the Unix/Linux command line is a surprisingly robust platform, that is very tolerant of being accessed in a variety of unusual ways. It takes some configuring and there is a learning curve, but once you're comfortable, you can get an astounding amount of work done. 

### How?

Lets revisit my original list of tasks, and break each one of them out over a serial terminal. Keep in mind that every machine on this list will have access to these applications over a wireless connection, so later when we are rating the various merits of the individual machines, we will lump their ability to do all of these tasks via Serial connection in to a single score. 

**Writing:** Nano, Vi, Emacs, Ed, Mp, Wordgrinder... There are a plethora of highly expandable, widely loved text editors and word processors available for the linux command line. The majority of them are fully interactive, and can be used from every computer on our list. 

**Email:** I use Mutt as my primary email client. I've also heard good things about pine, and I'm sure there are others. 

**Live Chat:** Shared unix servers invented live chat. There are dozens of services, from talk to IRC to XMPP. I prefer to use Finch and irssi, but there are literally hundreds of options. For years I swore by nAIM, but with the closure of AOL Instant Messenger I'd be surprised if it still works. 

**Research:** My research comes mostly from the web and from gopher. For the web theres Links, Elinks, Links2, Lynx, w3m, and I'm sure emacs has a browser mode. For gopher theres Gopher, lynx, w3m, and I'm sure emacs has a gopher mode. 

**Graphic Design:** It's easy to do graphic design from the commandline! Haha just kidding. I'll occasionally do some basic layout in HTML and CSS, or Latex but I recognize that some things just need graphics. 

**Publishing:** I publish this website using Jekyll from the command line. I manage dozens of other websites through other commandline means, sometimes by shelling in to the server and editing files directly in production (this is bad) or by updating my local copy and then pushing a new build (I'm told this is better.) If I have print documents ready to go in to publication, I can start a print run from the command line as well. 

**Development:** Pretty much all of my development is done using the same tools that I write in. That is to say that it all happens at the command line. I write PHP web apps, bash, lua, and python scripts, and all kinds of other fun stuff. For things that only require a simple UI, working from the command line saves steps. 

**Data entry:** Can you do data entry from the commandline? You betcha! There are CLI interfaces for most major databases, or you can rig up a custom application (in bash, or php, or lua, or python, or perl) to interface with the database for your users. 

**Calendar:** Sure, why not? Interact with google calendar through gcalcli. 

**Music:** You betcha! When I was using my Tandy 100 as my main computer, I had the server hooked up to my home stereo. I'd control the music for the whole house using cmus, which is still my favorite music player. 

**Mastodon:** There are a couple of Mastodon apps for the linux command line, and they are steadily getting better. There's also an IRC bridge and an emacs mode. 

**Books:** I mostly keep my library in epub, which I can convert to html and read with any of the many CLI web browsers using pandoc. I have that process aliased to a command called "read" so in practice I just type "read house-of-leaves.epub" and then I don't have to worry about anything else. 

**Movies:** The command line is not a great place for watching movies, but [it can be done](https://www.howtogeek.com/howto/linux/stupid-geek-tricks-watch-movies-in-your-linux-terminal-window/). If this is something you're seriously considering, stop it, and read the section on TVs instead.

**Podcasts:** I mostly do podcasts on my phone, and I've never looked for a CLI podcast app. I'm sure they exist, but keep in mind that the audio would play back on the Server, and not locally. 

**SSH/RDP/VNC:** I can manage my VPN connections and initiate SSH sessions from the command line. If what I'm doing actually requires RDP or VNC I have to move to a graphical terminal. 

**todo list:** [todo.sh](http://todotxt.org/)

**games (playing):** Yes, there are dozens of games for the command line, including the BSD games package. You can also connect to MUDs, play infocom games and other text adventures, and even play [multiplayer lightcycle racing](http://sshtron.zachlatta.com/). Mostly, that's a topic for another article. 

**Games (writing):** Sure, you can write games as well as you can write anything else, but if you want graphics look elsewhere. 

# Putting the pieces together

## Apple IIc

![By Bilby (Own work) [CC BY 3.0 (http://creativecommons.org/licenses/by/3.0)], via Wikimedia Commons]({{site.baseurl}}/images/1024px-Apple_IIc_with_monitor.jpg)

##### By Bilby (Own work) [CC BY 3.0 (http://creativecommons.org/licenses/by/3.0)], via Wikimedia Commons

### What?

The Apple IIc was Apple's compact version of the Apple IIe. It's a small, self contained computer, with a fair amount of power and a great industrial design. 

### Why?

It was seeing an Apple IIc in person for the first time recently that started me down this path again. The IIc is not a particularly important or impressive computer in terms of performance. It's essentially just an Apple IIe in a smaller case, and with some integrated peripherals. For me, what makes it stand out are two key features: 

1) It's pretty dern power efficient, drawing 18 watts on average (without a screen.) While that's more than, say, a Raspberry Pi, it's so much less than a) most other vintage computers, b) most modern computers. 

2) It was produced right in the moment when Apple decided to embrace svelte industrial design for the first time (a trend they would return to again and again.) It is a small and unassuming package, and clearly a product of the 1980s (19a0s?), but it has an *almost* timeless look to it, as well. 

Beyond that, it has a few more things going for it. Namely, it has a standard serial port built in, it has composite video out (for connecting to those TVs!) and modern hardware readily available to give it access to [Solid State Storage](https://www.bigmessowires.com/shop/product/floppy-emu-model-b/) and [modern monitors](http://www.a2heaven.com/webshop/index.php?rt=product/product&product_id=135). It loads to Applesoft BASIC which is widely documented and easy to use, and has multiple (good/interesting) graphics modes. It's FAST (for the time) and has a lot of RAM (for the time) and a huge software library (for any time.) 

### How?

**Serial Terminal** Use the Apple IIc as a terminal connected to a modern linux machine either via a null modem cable or a serial-to-bluetooth or serial-to-wifi adapter. The Apple IIc can display 80 columns of text, which makes it an ideal candidate for serving as a [Thin Client](https://en.wikipedia.org/wiki/Thin_client) in this fashion. 

Importantly, a wifi connection would enable multiple machines to share a single modern computer as an application server. Dozens, if not hundred, of concurrent users could get by on a single Raspberry Pi. 

**As a Stand alone computer** The same null modem/wireless serial setup can be combined with vintage programs from the Apple II library or newly written/custom software for the Apple II to enable it to serve as a Word Processor, Gopher/Web browser, BBS browser/server, or pretty much anything you can imagine, while still interfacing with a modern networked world. 

The Apple IIc (and later the IIc Plus) is a fast machine, compared to many of it's contemporaries. It has a lot of RAM, compared to it's contemporaries, and it can be put in to service as an excellent addition to your digital arsenal. 

Specifically, I could see the IIc serving as the interface to a Point of Sale system or the front-end for a custom database driven application. Its variety of hardware I/O, and the low level access to the hardware available from the machine combine to also make it an attractive choice for home automation tasks, or other projects that require directly interfacing with external hardware (much like a modern microcontroller, but arguably more capable and certainly easier to interact with). 

And I know the BBS line sound like a throwaway comment. It's not. I don't think we'll get to it in this post, but BBS connections can be a lot of fun, and super useful, if handled correctly. 

**A game console** There is a [HUGE library of games available for the Apple II](https://archive.org/details/apple_ii_library_4am), and the IIc is compatible with very nearly all of them. It might not be the most professional choice in the world, but the Apple IIc is hard to beat as a retro game console. 

**Development Environment** The Apple II line runs Applesoft BASIC which is a derivative of Microsoft BASIC which became QuickBASIC and GW-BASIC and BASICA and... well, basically programs that will run in BASIC on the Apple II can either run or be ported to run on many computers without a lot of fuss. Additionally there are Apple II emulators for dozens of computers, and even one that will [run in modern web browsers](https://www.scullinsteel.com/apple2/#hhgttg). 

![screenshot (4).jpeg]({{site.baseurl}}/images/screenshot (4).jpeg)

To me, that makes the Apple II an attractive choice as a development platform, with a set of strengths and quirks that keep it interesting and fulfilling. 

### Scorecard

Keep in mind that the Apple IIc can serve as a wireless serial terminal to handle all of the tasks we outlined above. Beyond that, here's a quick rundown of how it performs (if I've left something off, it's because it shouldn't be attempted on an Apple II. If I'm not sure, I'll indicate that.) 

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

**Publishing:** ?/5
I'm not aware of any viable page layout software for print publishing, nor of drivers for modern printers. Certainly vintage printers exist, and I'm sure there's some for of page layout software. 

**Development:** 3/5
No IDEs, but a good built in language and few bugs or physical constraints. 

**Data entry:** 4/5
Good built in programming language, wireless networking, and a high (text) resolution mean that this is a perfect target for data entry. 

**Calendar:** 0/5
No real time clock = no calendar. 

**Books:** 0/5
While it might be possible to rig up an ebook reader, why would you? 

**Movies:** 0/5
No video playback.

**todo list:** 3/5
It would be possible to cobble together a decent to-do list manager in BASIC, that syncs back to our central file server, but it would probably be better to do this through todo.sh on your application server. 

**Games (playing):** 5/5
Huge library of great games.

**Games (writing):** 3/5
Is a great platform for playing games, but it does not provide many tools for creating them. That being said, Applesoft BASIC is a decent, reasonably fast platform, and does not feel limiting. 

**Serial Terminal:** 5/5
Wireless, no adapters, fast, high resolution. Hard to beat. 

## Tandy 102 // Olivetti m10

### What?

![15635.jpg]({{site.baseurl}}/images/15635.jpg)

The first truly portable computer! Released under a dozen different names, with stylistic changes between each model, this cutie will run for weeks (months?) on a set of AA batteries. It's got a built in serial port, a good keyboard, and a screen that's just big enough to get stuff done. 

### Why?

I used a Tandy 102 for several hours a day for about two years. It's a Great computer, and I'd still be using mine if it hadn't developed some display issues. It is small enough and light enough and sturdy enough to toss in a bag and take with you on the road. The memory is large enough to hold a few dozen pages at a time. It's easy to interact with modern computers (provided you have the right cables) and it'll last for around a month of daily use on a set of rechargeable AAs. 

It's very nearly the perfect laptop. Plus the Olivetti version is one of the cutest computers I've seen in my whole life. 

It's also popular in the HAM radio community for doing SDR and packetBBSs, I've heard. 

### How?

The TRS-80 Model 100/Tandy 102/Olivetti m10 is useful to a modern office in exactly two ways: 

- As a wireless serial terminal (over BT or wifi, doesn't matter.) The Tandy's screen displays just barely enough text to do useful things. 
- As a distraction free portable word processor (although even this is easier and more fun if you're just using it as a serial terminal to a Linux box running your favorite text editor.) 

Having used this one pretty extensively, I feel comfortable saying that you should *not* try to use these computers as stand alone machines. They don't have the horsepower. They don't have the RAM. They were never designed to live on their own. 

But, as a wireless terminal connecting back to a raspberry pi (or an android phone! or a remote server) it can really feel magical. The screen has decent contrast. You can mostly read it in the sun. I've used mine for email, chat, and some basic web/gopher browsing. I've written blog posts on it, and published websites. I've played Zork. Heck, I've solved serious production issues on client servers from the park, with the Tandy connected to my phone's hotspot over wifi, and my phone providing a VPN connection through which I could telnet to my server, and SSH from my server to the client environment. 

It is a full fledged computer. You can do spreadsheets or write your own programs directly on the device. Some people really get a kick out of that. I never did, but I'm grateful for the ways that they continue to extend it. 

### Scorecard

The Tandy 102 can serve as a wireless serial terminal to handle all of the tasks we outlined above. It does this really well, and is a lot of fun to use for that purpose. Beyond that, it's also a pretty great machine for writing. 

**Writing:** 4/5
Small screen makes editing difficult, but the keyboard feels good to type on, and you can take it anywhere. 

**Serial Terminal:** 4/5
I want to give this computer a 5 because it's so much FUN to use as a serial terminal, but it's a little tricky to do the initial setup. I've only done it a few times, but I'll try and put a guide together soon. Also, the small screen and nonstandard font results in some difficulty when interacting with any complex user interfaces, which is a real shame because it's Fun to use this computer. 

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
'

### Scorecard

Keep in mind that these compact macs can serve as a wireless serial terminal to handle all of the tasks we outlined above. Beyond that, here's a quick rundown of how it performs (if I've left something off, it's because it shouldn't be attempted on a classic Mac.) 

**Writing:**  5/5
Default keyboard isn't bad, and plenty of third party upgrades are available. Can write directly on the machine and transfer files via flash media or wirelessly. There are some seriously stellar word processors for the Mac.

**Email:** 3/5
You can set up an email account on a BBS, or use a vintage pop3/smtp email client, and configure another machine on your network to serve as an email proxy to interface with your IMAP inbox. It's not super straightforward to set up, but once it's done it works well.  

**Live Chat:** 4/5
MacIRC works well and is easy to use. You can configure your IRC server to act as a gateway to other chat services. Other IRC and chat applications also exist, but I've never tried them. 

**Research:** 3/5 
Can access BBSs directly. Can run a Gopher browser. I do not recommend running a web browser (but it can be done.)  

**Graphic Design:** 3/5 
Several vintage graphics packages are available, a few of them even support modern file formats! But you're still stuck in monochrome, and the screen is still pretty low resolution. I've seen the classic macs used for some serious layout work, but not a lot of more involved design. 

**Publishing:** 4/5
Lots of good page layout and typesetting software. Plenty of good fonts. Can't directly interface with modern printers, but can export documents in modern file formats. Also, Fun to use. 

**Development:** 5/5 (several hundred out of five) 
If you haven't caught on, I love hypercard. There are also many other IDEs and development environments available, but I don't know why you'd use them when Hypercard exists. 

**Data entry:** 3/5
Small screen, better for other tasks. Can certainly be used for data entry, but that's a wasted potential, in my opinion. (On the other hand, your custom Hypercard application could serve as a front end to your database, or a way to pull reports, and then I would applaud.)  

**Calendar:** 3/5
Works well enough, but not my first choice. 

**Books:** 0/5
While it might be possible to rig up an ebook reader, why would you? 

**Movies:** 0/5
No video playback.

**todo list:** 3/5
It would be possible to build an excellent to-do list manager with hypercard, that syncs back to our central file server. But it would probably still be better to do this through todo.sh on your application server. 

**Games (playing):** 4/5
Good sized library of not bad games.

**Games (writing):** 3/5
I've never written a game on a Mac. I imagine it would be pretty easy (and there's always Hypercard~!) 

**Serial Terminal:** 4/5
Wireless, needs an adapter, fast. 

## HP 200 LX

### What?

![Hp200lx,_open.jpg]({{site.baseurl}}/images/Hp200lx,_open.jpg)

My favorite computer on this list, the HP 200LX is a weird little relic. It was originally released in 1994, and is the third in a line of **palmtop** computers released by HP in the early 90s. It's an IBM PC Compatible DOS computer, built around a 186 processor with a greyscale CGA compatible screen and a whopping 2MB of RAM, it will run for weeks on 2 AA batteries. (No really, I've done it.) 

### Why?

Again, because it's heckin' awesome. It's got a sunlight readable screen, the largest software library of any computer we've discussed so far, built in support for PCMCIA storage devices (and therefore CF cards.) It runs DOS, which is my favorite OS of the 1980s, if only because it's the one I've had the most direct experience with. 

Also, it has a great calendar app, a good set of programs to sync with (more) modern computers, and a tiny RS-232 compatible serial port. 

### How?

**ebook reader** it's a sunlight readable, handheld clamshell device that'll run forever on a pair of rechargeable AAs. Couple it with Vertical Reader (or VertReader or VR) by Giles Kohl and you've got yourself the best little ebook reader. I used mine to read A Princess of Mars at the beach in 2007. 

**Standalone** It's a palmtop computer! With a CF card slot that you can use to transfer files to from another computer. There are hundreds of applications written specifically for this machine, and it is compatible with (tens of) thousands of DOS applications. Add an RS-232 Wifi modem and It'll run SSH (slowly, but it'll do it) and a web browser (ARACHNE) and a gopher browser and all kinds of other neat stuff. 

It'll play Zork, it'll manage your email. It'll run Windows 3.1 or GEM or ... Look, I'll do an article about DOS in general and the HP LX line specifically in a few weeks. As a standalone computer, it's surprisingly powerful and fun. 

**Serial Terminal** Yep! This one can be a wireless serial terminal too. You gotta do some fancy stuff to get a wireless adapter to plug directly in without an additional cable, but it'll work. The keyboard is a little tight, and the addition of the numberpad was a Big Mistake IMO, but it's still a functional little machine to use while you're kickin' it on the couch. 

**Dev Environment** It runs DOS. You know what else runs DOS? Everything, thanks to DOSBox. It also has compilers available for dozens of languages, and my favorite text editor (edit.exe).

**PDA** I know that PDAs are passé in the era of the smartphone but hear me out. They are wonderful. Managing your calendar, your to-do list, and your contacts from a device that is also a full fledged computer and isn't pretending to be a phone is pretty wonderful. Using the same device to manage email, social media, and chat can also be pretty great. About the only things it won't do are take calls and media (which, incidentally, are things my phone is great at.)

### Scorecard

Keep in mind that the 200LX can serve as a wireless serial terminal to handle all of the tasks we outlined above. It performs at this job admirably, especially considering it's small size and battery power. Beyond that, here's a quick rundown of how it performs (if I've left something off, it's because it doesn't really work here.) 

**Writing:**  3/5
GREAT software meets a decidedly mediocre keyboard. Well, no. That's unfair. 

The keyboard is not bad to use. It's very clicky and tactile. I liked typing on it, mostly. It's just the damn number pad I take an issue with. The numberpad should have been omitted. 

Either way, it's a handheld, you'll be typing with your thumbs. It works, but it's not the best experience. 

**Email:** 3/5
You can set up an email account on a BBS, or use a vintage pop3/smtp email client, and configure another machine on your network to serve as an email proxy to interface with your IMAP inbox. It's not super straightforward to set up, but once it's done it works well.  

**Live Chat:** 4/5
There are multiple IRC clients. You can configure your IRC server to act as a gateway to other chat services. There are multiple XMPP clients. 

**Research:** 3/5 
Can access BBSs directly. Can run a Gopher browser. Can run Arachne web browser. Seeing the web through a DOS web browser is... something else, but it can be done.   

**Graphic Design:** 2/5 
Tiny, low resolution, 4-color CGA crushed to grayscale screen. Don't do this to yourself. 

**Publishing:** 4/5
Lots of good page layout and typesetting software. Can't directly interface with modern printers, but can export documents in modern file formats, and has easy removable storage. 

**Development:** 4/5  
Lots of development packages available. None of them as good as hypercard, but some of them come close. Has compilers for nearly every language under the sun, and emulators on every modern platform. 

**Data entry:** 4/5
The screen is small and the keyboard is as little awkward, but it's also a handheld machine with a wifi connection and a keyboard that works well with thumbs. Rig yourself up a couple of .bat files to handle your I/O and get to work. 

**Calendar:** 5/5
Excellent, carefully thought through calendar. 

**Books:** 5/5
Was my favorite ebook reader until I got an ebook reader with a back-lite. Doesn't support a ton of file formats, but that's why devs made Pandoc 

**Movies:** 0/5
No video playback.

**todo list:** 4/5
It's a PDA! It has a good built in to-do list manager, that syncs with outlook if that's your thing. 

**Games (playing):** 4/5
Good sized library of not bad games. Some are hard to see in greyscale, others run a little slowly because it's essentially a first gen IBM PC in the palm of your hand and of course that means it's a little slow. 

**Games (writing):** 3/5
I learned to program on this machine, and wrote several bad games for it. It's not too hard. 

**Serial Terminal:** 4/5
Wireless, simple pass through adapter, handheld. 

## Atari

### What?

The Atari STacy and ST BOOK are laptops from the late 80s and early 90s. Both of them had greyscale screens. They are both members of the Atari ST family, which was Atari's entry in to the 16 bit home computer market.

The ST family ran Atari TOS under the hood, meaning a GUI and file manager (called GEM) that looks a lot like a classic mac. It could read and write from DOS compatible floppy disks. They have a large library of software, though not as large as the Mac or DOS library, and a surprisingly strong collection of real time music making applications. 

### Why?

The ST BOOK is the computer from this line that I'd be most interested in incorporating in to our office. The ST BOOK was pretty lightweight, could run on AAs, and had surprisingly good battery life (it draws about 20 watts of power when in use.) It has a sunlight readable, non-backlit screen, no internal floppy drive (I consider that a plus!), and an interesting physical profile. Additionally, it had a pretty great set of interfaces: 

- MIDI x 2
- Serial Port x 1
- Parallel port x 1
- FDD/ACSI x 1 (can be converted to SCSI with a simple adapter)

All of that was rounded out with an internal HDD, mounted with a standard 2.5" IDE cable. That means that we can buy off the shelf IDE->CF or IDE->SD adapters to replace the moving hard drive with a solid state disk, resulting in a laptop with even better battery life, larger storage, and no internal moving parts. 

Various European vendors also sell add ons that can add USB mass storage, CF cards, or SD cards through the FDD/ACSI port found on most ST computers. Since TOS used an MSDOS compatible disk format, that means that you can swap these external storage disks with any modern computer, as well as any vintage DOS or Windows computer (with the appropriate adapters.)

### How?

We've covered most of these Hows before. There is very little the ST line can do that is unique to the ST line beyond a couple of pieces of exclusive software. The ST line in general would excel in all the same places that a DOS machine or a compact Macintosh would excel (minus multi-tasking and hypercard, of course.) The ST Book would come with the advantage of a small, light formfactor and true wireless operation. Where this platform stands out, is in music production with lots of synth and tracker software and 2 MIDI ports, even on the ST BOOK, the ST line is right at home in a studio. 

If you're not making music, the ST can still hold it's own as a standalone machine, and as a serial terminal to a more modern machine. It can access BBSs and Gopher servers and handle email and basic web browsing. Plus, it has a nice keyboard and it looks neat. 

### Scorecard

Keep in mind that these Ataris can serve as wireless serial terminals to handle all of the tasks we outlined above. Beyond that, here's a quick rundown of how it performs (if I've left something off, it's because it shouldn't be attempted on an ST.) 

**Writing:**  4/5
Decent keyboards. Can write directly on the machine and transfer files via flash media or wirelessly. There are pretty good wordproccessors for the ST family.

**Email:** ??/5
Never tried it, but I assume it would need an IMAP to POP proxy, or a BBS mail account. 

**Live Chat:** 4?/5
It appears there are lots of live chat applications available, but I've never used any of them. 

**Research:** 3/5 
Can access BBSs directly. Can run a Gopher browser. Has access to a basic web browser, but it's a *very* basic web browser.  

**Graphic Design:** 3/5 
Several vintage graphics packages are available, a few of them even support modern file formats! But you're still stuck in monochrome. On the plus side, the screen runs at an almost modern resolution! 

**Publishing:** 4/5
Some good page layout and typesetting software. A few good fonts. Can't directly interface with modern printers, but can export documents in modern compatible file formats. Also,  

**Development:** 3/5 
No more difficult to develop for than DOS or the Apple II, but fewer folks on the receiving end to run your applications, as emulators are further between.  

**Data entry:** 4/5
Good keyboard, good screen, can run custom applications. Perfect candidate for data entry. 

**Calendar:** 3/5
Works well enough, but not my first choice. 

**Books:** 0/5
While it might be possible to rig up an ebook reader, why would you? 

**Movies:** 0/5
No video playback.

**Music** 3/5
Can't play back your MP3s, but can be used to Make music. One of the earliest computers to feature a soft-synth.

**todo list:** 2/5
I've seen a few todo list managers, but none of them impressed me.  

**Games (playing):** 3/5
Some people swear by the ST as a gaming machine, but I've never understood it.

**Games (writing):** 3/5
I've never written a game on an ST. I imagine it would be no more difficult than DOS.  

**Serial Terminal:** 5/5
Wireless, no adapters, fast. Hard to beat. 

## G4 eMac, G3 iBook, G5 iMac

### What?

Apple Macs from the early 00s. The newest machines on this list. I'm grouping them together because for practical purposes they are very similar. I will take a moment to describe their few differences: 

**G4 eMac** this was an iMac made for the educational market, and built around a CRT. It's big and bulbous and looks for all the world like a product of Braun circa 1965. It has a 16" screen running at 1280 x 960, and can support up to 1GB of ram. It has built in wifi, speakers, a DVD/CD combo drive, and can support up to Mac OS 10.5 

It's a heavy monster, and were it not for the fact that it's design fits my desired aesthetic so well, I wouldn't be considering it. It's also a surprisingly powerful and capable machine. 

**iBook G3** slightly older than the eMac, this is a laptop originally launched in 1999. Known for it's candyshell design, the iBook G3 feels less like a modern machine in use than either the emac or the G5 iMac. The system is equipped with an 800x600 display, and shipped with 64MB of RAM (expandable up to 512MB.) It originally ran Mac OS 9, but can be upgraded up to 10.3. It features USB 1.1 ports, firewire, and wifi. 

Compared to the eMac or the G5, the iBook begins to look and feel like a toy. It isn't, and it has a few tricks up it's sleeve that we'll discuss in a moment. 

**iMac G5** It almost feels like cheating to put the G5 on this list. Almost. But the things that make the g3 and the g4 attractive to me for this purpose apply just as much to the g5, while also giving us the benefit of a much more powerful computer. 

When you think white plastic iMac, you think of the g5. With a 20", 1680 × 1050 display, a 2.1 GHz powerPC processor, up to 2GB of RAM, and up to 500GB HDD, the G5 iMac is very nearly a modern computer. If it had an intel chip inside (like the model that replaced it), it likely would have continued to receive updates trough 2011 or later. As is, though, it got left in the dust by the shifting tides of corporate favor. 

For us, that's great news. It's a beautiful machine, with more juice than 10 of pretty much anything else on this list. It runs a decidedly modern operating system, and has access to a large software library. 

### Why?

The Why for this one is almost too easy. All PowerPC macs can run classic Mac software. That means that every computer in this group has access to Hypercard. Plus, intrepid hackers are still out there building modern software for OS X 10.5 and some even build for Mac OS 9.x. Plus each of them has a decidedly unique and nearly iconic look. 

### How?

Every computer in this group can be used in most of the same ways you would use a brand new computer (although you may occasionally get frustrated using the iBook in this fashion) while also providing access to a wealth of vintage software and the best non-technical application development platform ever made. 

Beyond that, Mac OS 9 (available on the iBook) uses a Cooperative Multitasking model. That means that it's effectively single tasking, relying on the foreground application to pass control to other applications. For a lot of things, this is pretty shitty, but it means that the running application gets unprecedented access to system resources. That means that tasks which seem to creak under OS X on the iBook or eMac will feel Much more responsive under OS 9. 

The eMac G4 or the iMac G5 would make a great media player, audio editor, graphics editor, or even video editor. They have modern web browsers, and support modern encryption protocols. I learned graphic design, audio engineering, and video editing on an eMac. 

The iBook would make a solid audio workstation under OS 9. It would make a usable, if slow, imitation of a modern computer under OS X. Under either OS, we could treat the iBook like one of our older machines. Using it as a serial terminal, focusing on it's strengths (hypercard, audio editing) and offloading more processor intensive tasks to a newer machine. 

Uisng the iBook with OS X we could run locally many of the same applications that we would access remotely from a serial terminal. That is to say that OS X gives us direct access to a Unix command line, which would enable us to access BBSs, email, web browsers, and a whole mess of other command line applications, without having to rely on a mainframe. 

Plus, you know, there's Hypercard. 

### Scorecard

Keep in mind that these macs are only a few generations old. They have wifi built in, and feature a slew of modern connectivity options. They can certainly serve as a wireless serial terminal to handle all of the tasks we outlined above, but they can also run all of those CLI applications locally.

Beyond that, here's a quick rundown of how they perform.

**Writing:**  4/5
Good software, generally good keyboards. Not as fun or as simple as others on the list, but 100% serviceable. Can write directly on the machine and transfer files via flash media or wirelessly. Basically just like using a modern computer, but honestly probably faster in practice. 

**Email:** 5/5
They'll all run a fairly modern web browser and email client. 

**Live Chat:** 5/5
Software for all the major networks and all the minor networks and most of the defunct networks.  

**Research:** 5/5 
Can access BBSs directly. Can run a Gopher browser. Has a port of firefox with many (but not all) of the current features. 

**Graphic Design:** 5/5 
I learned Creative Suite on an iMac G5. Maybe don't try graphic design on the iBook, but the other two are good to go. 

**Publishing:** 5/5
Lots of good page layout and typesetting software. Plenty of good fonts. Can directly interface with modern printers, and can export documents in modern file formats. 

**Development:** 5/5 
If you haven't caught on, I love hypercard. There are also many other IDEs and development environments available, but I don't know why you'd use them when Hypercard exists. 

**Data entry:** 5/5
Better for other tasks, but can certainly be used for data entry. No reason it won't perform above and beyond. 

**Calendar:** 4/5
Works well enough.

**Books:** 2/5
Several ebook readers exist, but reading on a desktop or laptop isn't a lot of fun. 

**Movies:** 5/5
The iBook might struggle a little bit, but even the iBook will handle SD movie playback. The eMac and iMac can decode 720p files without any trouble, and both would make a decent SD video editing rig. 

**Music:**  5/5
The iBook, running OS 9, has access to plethora of snappy and robust DAWs. All three under OS X can run several reasonably modern audio editors. All of them can handle podcasts. All of them can do music playback. 

**todo list:** 5/5
Can run todo.sh, and sync with your master copy.  

**Games (playing):** 3/5
Good sized library of not bad games.

**Games (writing):** 3/5
I've never written a game on a Mac. I imagine it would be pretty easy (and there's always Hypercard~!) 

**Serial Terminal:** 5/5
Built in Wifi, no adapters required. 

## Phones

### What?

![contempra.jpg]({{site.baseurl}}/images/contempra.jpg)

Vintage desk phones! The big ol' clunky ones from the 40s! The space age ones from the 70s! The more unique looking the better. 

### Why?

Because SIP phones are dull *and* expensive, and these will work just as well, and be way more fun. These vintage desk phones will compliment our aesthetic perfectly. 

### How?

With [Asterisk](https://en.wikipedia.org/wiki/Asterisk_(PBX)) along with a channel bank like the CISCO PAP2T or an Obihai OBi110 or similar. 

## TVs and Monitors

### What?

![JVCVideoSphereVideoCapsuleTogether.jpg]({{site.baseurl}}/images/JVCVideoSphereVideoCapsuleTogether.jpg)

Old TVs! Like the Philco Predicta or the JVC Videosphere or other more common but still spacey looking TVs. 

### Why?

Because they look awesome! Because they are a pain to recycle so we might as well re-use them. Because they are begging to be made in to video phones. 

### How?

**Videophone**
Hook a computer up to one of these, and mount a little camera and mic around it somewhere and it becomes a video phone, that will 100% STUN your clients when they see it. I had a simple setup (not even particularly elegant, literally just a raspberry pi with a mouse and keyboard and webcam) set up for a few months, and everyone that saw me videoconferencing on it stopped and stared. 

Now imagine I had been [using one of these](https://stellartv.files.wordpress.com/2014/09/dscn4509.jpg), instead of a mid-80s luggable. Seriously, it's the best. 

**Monitor**
Most vintage computers need a monitor and have a composite video output. Most TVs can be a monitor and have (or can be rigged to take) a composite video input. Combine these two facts for fun and profit. 

**Video Player** 
While most older computers can't actually play videos, they CAN (as we have well established) serve as serial terminals. Set up a media player attached directly to one of these TVs or using the broadcast method described at the top of the page, and toss together some bash scripts to display the available files and control playback (incorporate UPnP to enable folks on your local network to be able to control playback from their phones as well.s 

If you go the broadcast route, you get to have the benefit of a clean wireless setup, and multiple TVs (including handhelds!) displaying the movie, tv show, game, or other content of your choice. Again, it can lead to some really impressive moments (especially if you're controlling all the playback from an Apple IIc or an Tandy 100.) 

**(The same idea discussed here for a video player can also work with an old stereo as a music player.)**

## Other potential machines

Of course, the above are far from the only vintage (or vintage adjacent) computers that'd I'd consider. They're just the ones on my mind right now. Here's a quick rundown of some other machines I've considered, or learned about recently and will be exploring.  

### c64

My favorite vintage computer! Unfortunately, it's not sexy and it's not really good for much beyond gaming (when compared to the other computers on this list.) 

### Amiga!

Commodore's 16 bit computers were AMAZING. But they never made a portable unit or a compact unit and the full sized units are power hungry monsters. Add to that the fact that I'm not super familiar with the software available for them. 

If I found one, I'd look for a way to integrate it, but I don't know that I'd go looking for one right now. 

On the other hand, I know that the Amiga had an add-on card (the video toaster) that enabled it to be a strong SD video processing rig. With the right hardware and software, and a decent vintage camera, the Amiga and produce SD broadcast quality footage. The temptation to hunt one of those down is metered by the fact that they still cost about 1000 dollars, and the fact that I don't have time to get in to 3D animation and video production right now. (but hey, give me a few months and $1000.) 

### Armiga

An Amiga, rebuilt on ARM for gaming mostly. Newly produced, legal emulator built around a raspberry pi or adjacent. 

On one hand, I'd love to have one! On the other hand, I need to know way more about the Amiga and it's abilities, and the strengths and limitations of the Armiga before I consider springing for one. 

### Cambridge Z88

Looks like a Tandy 102, but a little newer, with a better screen, a worse keyboard, and fewer connectivity options. 

It's high on my list, because Douglas Adams used one while writing Last Chance to See, and I love Mr. Adams, but also I'm not sure if it could be easily brought in to my workflow (specifically, it seems that the serial port is non-standard, and it does not use any modern storage.) 

### Risc OS on Pi

Not exactly vintage, but running the OS from the Acorn Archimedes on the Raspberry Pi. It's not an emulator, it's am actual OS. 

They don't currently have Wifi support. Once they do, I'll install and get RISC OS worked in to my daily workflow. 

### Psion Series 5

!! What a great little thing. Two things are keeping it off the list: 1) The screen is apparently not wonderful, especially with the backlight off. 2) I [backed the project](https://www.indiegogo.com/projects/gemini-pda-android-linux-keyboard-mobile-device-phone) for it's modern successor which will allegedly ship this month. 

It has a lot in it's favor though: Great keyboard. Optional backlight. Native CF card support. Modern OS available. A semi-standard serial port that can be connected to our wireless modem with only a minimum of elbow grease. 

And they're pretty cheap, averaging less than $100 on ebay the last time I checked. It'll be hard not to buy one soon. 

------

## A fiction, to tie it all together

*Every character in this thing is a reflection of myself. If I'm too harsh on Drew, it's because I see myself in his position now.* 

Drew, a young business owner, is having coffee at his local haunt in the trendy historic district of the trendy suburb of the trendy but not too expensive city. There is a lot of exposed brick around him, and kids dicking around on tablets and smartphones. He looks and feels a little ancient as he adjusts his too expensive headphones and peers over the top of his painfully bland brushed aluminum laptop. 

Wanting to appear less like a man slowly aging out of his own demographic, drew takes a long slow sip of his too expensive coffee, closes his eyes, and leans back. On the ceiling, there is a flyer. The ceiling is very far away, and the flyer is a jumble of too many words. Drew's eyes have gotten worse since the last time he went to the eye doctor, and to him the flyer is almost impossible to read. At the bottom, in larger letters, it says "Basically, if you need help, we're four doors down. Look for the weird." 

'A flyer on the ceiling of a coffee shop that says "look for the weird." How could I pass that up?' he thinks. Hesitantly he gathers his things together and steps out the door. Instinctively, he turns to the right back towards the little city's town-square and park. He watches the doors and counts. There are three. There was not a fourth. 

Drew is disappointed, and now he feels foolish. He turns to go back towards the coffee shop before realizing that the little side street that plays host to Hot Beans Coffee Roasters does not in fact end at their door. That's just the furthest he'd ever been down this street. He walks past the coffee shop, past an empty store front, past a hair salon, past a church for a religion he was sure he'd never heard of, and then he noticed another door recessed in the wall, opening on to a staircase. 

The door is black, or maybe purple, with stars across the bottom. The top portion features a big, highly reflective pane of glass. The lettering on the glass reads "Space Age Ideas: Wizards of the Electronic Age. We help, We consult, We build things, Come inside!" 

He waffles for a moment, tugging at the strap of his shoulder bag. As he stands there, the door clicks open. A voice from upstairs says "we have video games!" 

With that, he has no excuse. He steps through the door, which closes itself behind him, and climbs the stairs. He's in an industrial space. It has the same trendy exposed brick, worn wood, and bare metal look, but it feels mostly earnest as the 200 year old stairs creek slightly under his weight.  

He emerges from the staircase in to an office. He thinks it's an office, at least. There are a few people lounging around on couches and slightly pretentious mid-century modern chairs, and 6 or 7 people on various desks scattered throughout the long narrow room. On several of the desks he spots various beautiful old televisions; Some of them are displaying text, a few appear to have games he doesn't recognize or TV shows he hasn't seen. 

He pauses to take it all in, waiting for someone to acknowledge his entrance. Clearly some these people were working, he thought, but on what he could not begin to fathom. Their machines seemed to clearly be barely functional antiques, and yet every last one of them had an aire of the future to it. As he tries to reconcile all of this in his mind, he notices the robot. 

It isn't a large robot. It looks like a toy that might have been sold in the 1980s, but it moves with more grace than he expects. It rolls easily across the uneven wooden floor and stopped in front of him. It's head is another TV screen, bulbous like a spaceman's helmet, and there is a person's image displayed inside. 

"Hi, I'm Jerry!" the main inside the space helmet TV set says, "This is Space Age Ideas. What can we help you with today?" 

Drew stammered for a few seconds. "I uhh... I... I saw a flyer in the coffee shop and I couldn't really read it but I was feeling kind of down and the flyer said to come by if I needed help and then a voice said 'we have video games' and uh... what is this place?" he spat out all at once, the words tripping over one another. 

"Neat!" Jerry responds from his robot. "This is space age ideas! We're wizards of the electronic age, and we're here to help. What's your name?" 

"Drew"

"Drew, Give me a second, I'll have someone show you around." The screen flickered, and Jerry's face is replaced with an electronic smile. 

"Can I Help You?" the robot says in a shockingly synthetic voice. 

"N..No. I'm just waiting" Drew says, unsure of the correct etiquette for interacting with a robot. 

The bot turns around and wheels itself away, heading towards one of the doors at the back of the room that opens as it approaches. Drew catches a glimpse of dozens more robots waiting inside.  

A young woman sitting in one of the almost pretentious chairs, clearly rocking out with a pair of headphones that were remarkably similar to the ones Drew had so recently stowed in his bag, closes a small device about the size of a paperback book, places it on an end table, removes her headphones and walks towards him. 

"Are you Drew?" she says. 

"Yes, I am" he responds, more than a little embarrassed to be here. 

"Neat! I'm Dianne. Jerry asked me to show you around. Do you want to play some video games, watch a movie, or learn about the stuff we do?" 

"I... uhh... What?" 

"Great! We'll start with learning about the stuff we do. I'm sure you've heard the schpeal about helping and wizards. It's cute, but it's pretty meaningless. Here, follow me." 

They walk around the office, and she introduces Drew to people, and telling him about the projects they are working on. There is Jerry doing robotics on what appears to be an old black and white mac, John who builds websites on electronic typewriters, Cheryll who apparently publishes magazines and flyers with too many words, all jumbled together and cramped with the aide of what appears to be a pocket calculator, and several other people who's jobs appear to consist mostly of typing things in to the strangest computers Drew has ever seen. 

Drew is impressed by how quick everything seems to be, by how few wires he sees connecting things together, and by the sheer variety and beauty of the objects in the room. Mostly, though, he's impressed by how much Fun everyone seems to be having. 

"So, what do you do?" the young woman asks.

"Oh, I run a shop across town." Drew responded. 

"That's nice! But what do you do? Like, for fun? What do you make? What lights you on fire?" 

"I... uh... I have no idea." 

"Oh. That's not cool" Dianne said with a frown. "Do you like music?" she says, gesturing at her headphones. 

Drew stammers some more, and then pulls his nearly identical pair out of his bag. 

"You wanna hear the stuff I've been working on?" she says a little sheepishly. 

"Sure!" 

She plugs his headphones in to a table in the center of the room, picks up a small plastic box about the size of a paperback book, and opens it. He can see a small monochrome screen, and rows of tiny buttons. He starts to ask what this odd device could possibly be, but before he can find the words some strange and wonderful electronic music begins to trickle in to his headphones. 

Drew listens for a few minutes. He's impressed, and he says so. Dianne shows him over to her desk, where she has an array of old keyboards running in to a weird, clearly old, and therefore almost impossibly thin laptop running something that looks vaguely like an old macOS. She opens a tracker, plugs in his headphones, and they noodle for a few minutes.

The minutes slip in to hours, as Drew makes new friends and plays video games and makes music. Jerry comes over, in person, at one point and gives Drew a rundown of the features of his various robots, intimating that, indeed, they are built on chassis from toys made in the 1980s. Eventually, Cherryl thrusts a newly finished print zine in his hands and he flips through page after page of dense collages of words, confused and delighted. 

Suddenly the thought occurs to him that this place has got to make money somewhere, and everyone is too happy and relaxed for this to be the way that they do it. 

He looks for Dianne, and asks her. 

"Oh! Well, yeah. The big draw is "consulting" which in this case means teaching people things that help them solve problems, but beyond that we do all kinds of things. I mean we build robots for people and make websites for other people and write computer games and there's a crew in the back doing a TV show right now and we publish books and record..." she continues on like this for a few minutes "oh, and there's a tip jar by the door." 

"Do all of you work here?" 

She looks around for a moment "Work might be a strong word. A lot of us get paid to be here, either by Space Age Ideas directly--Like me--or through the work that we do while we're here. Everyone kicks in when they can to keep the doors open, and the place friendly. But this is just one office. Space Age Ideas is all over the world. Would you like to meet some of our other members?" 

Drew nods, and Dianne leads him to a large antique television sitting on a pedestal towards the back of the building. She pulls out her little pocket computer again, enters some archane incantation, and then a picture springs to life in front of him. 

He sees another office, shaped differently and filled with different people and different machines, but still clearly of a kind with the anachronistic timelessness of this place. 

"Where is that?" Drew says to Dianne. 

"Oh, We're in north Maryland" someone replies from within the screen. 

"Wait! Is he... Are we... Is this a video phone? Did you just walk me up to an antique video phone?" 

The man from north Maryland replies "Yeah, pretty much! It's neat right? I'm Steve. You new?" 

Drew and Steve and Dianne and various other people from both offices filter by the ancient TV and chat with one another. One of Jerry's robots rolls by in the Fredrick office, carrying a tray of magazines. A few people there pick one up and flip through it, one of them comes over to congratulate Cherryl on finishing her latest issue. 

For a moment, Drew struggles to understand what he's seen, and he can't shake the feeling that this is just magic. Slowly he remembers that things like The Internet, and network attached printers must exist even in this psudeo-timeless Eutopia. Even with that realization, as he looks around, he still feels like this is magic. 

As the day draws to a close, and the evening rises, Dianne gets Drew set up with a membership and offers him a handheld computer like hers to use until he has decided on his own workflow. Eventually, he leaves and makes his way back home. 

When he wakes up the next morning, he's uncertain that the place he has just visited could possibly exist. Tempted to shake it all off as a bad dream and an impending sense of ennui, he tries to push Space Age Ideas out of his mind as he gets ready to go. 

As he steps out the door, he notices a lump in his jacket pocket. He fishes it out, and finds Dianne's computer and Cherryl's magazine. On the back of the magazine, in the jumble of all the words too tightly spaced, his eyes fall on the phrase "it wasn't a dream." 

He smiles to himself, stows the computer in his pocket, and resolves to make something that feels like magic.
