---
layout: post
category: post
published: true
title: Reaching the World from Windows 3.1
---
I have an HP omnibook 300. It runs Windows 3.1 from ROM. It's about the coolest computer that was ever made: Almost exactly the size of a notebook (8.5x11.2x1.5" or so), instant on, no moving parts, stiff but reasonably satisfying keyboard (rubber domes, but decent ones), a non-backlit, sunlight readable, reflective TFT LCD and it runs for weeks of daily use on 4 rechargable AA batteries. I could talk about the computer for a while, but I'd rather talk about how I have been using it and how I want to use it in the future. (Tools are, after all, only as interesting as what we use them for.) 

My goal is to develop an offline first, asynchronous workflow that will allow me to interact with the world on my terms, at my pace, but won't prevent me from doing any of the things I find important. 

## Now

It is very nearly a single tasking machine, even though the included Windows 3.1 is technically capable of limited cooperative multitasking, the difficult to upgrade 2MB of RAM on the machine ensures that I am rarely doing two things on it. 

This has the unexpected benefit of making a great environment for writing, so I use the box to write a lot. I call it my ZineStation, because I use it to write the text that goes in to the zines I print, but it is also used for writing updates for my various websites, the scripts for [Expedition Sasquatch](https://expeditionsasquatch.org) and various other text projects. The things I write are saved to a compact flash card, which I can then stick in any number of other machines to post or email or process. 

I also use the box to write simple tools for me to use, often in qBasic or an old version of Python. My first computer ran Windows 3.1, and I cut my teeth there, and even though I know there are better tools for many jobs, the tools available to me in Windows 3.1 are often Good Enough for me to do what it is that I need to do. 

I've even managed to get a decent Desktop Publishing workflow going, and I produce a physical newsletter and a handful of pamphlets entirely on this machine. 


## Limitations

There are a lot of ways that this little box is decidedly living in the past, but not all of them are *bad*. Some of them, though, have proven to be annoying at one level or another: 

- No sound card, just a PC speaker
- No networking to speak of (we'll get to that.) 
- Removable storage is limited to very small cards 
- Useful and Interesting software for Windows 3.1 and DOS is getting hard and hard to fine, and what does exist tends to target powerful 486s and full color VGA (I'm guilty of this myself!) 
- No TLS or working SSH 

And there are a few other things that I've already got workarounds for or have resolved to fix. I'll list them anyway:

- I have grown accustomed to having the ability to query wikipedia and various other reference sources at will, but the Omnibook doesn't currently allow this 
- I frequently use the device to read RSS feeds, emails, etc. I have to remember to prepare these things in advance, and make a point to transfer them to the omnibook ahead of time. This means that, unless I manage to do it every morning "just in case", I'm often stuck with outdated info on the device 
- backups are entirely manual at the moment
- People stop and ask me about the box All The Time. People ask me lots of questions, that's not a big deal, I don't mind talking to people. But while I've been typing this, I've stopped to explain what the thing is Four Times, and this is in a place where I use this laptop several times a week (it's worse in new places.) 

## The future

Let's go over the things I already have solutions for, and then talk about my pie in the sky stuff. 

### Current solutions:

** Reference Material ** - I mostly use my phone for this, because that's the obvious solution, but I also don't like this! For now, I have an offline copy of most of wikipedia on my phone, and an old copy of microsoft encarta. These are both partial solutions, but they'll do for now. 

** RSS and Email ** - I came up with a pretty clever solution for this one, I think. I have a Raspberry Pi 0w. On reboot, it connects to any wifi network it recognizes in range (my home network, my phone's hotspot, the wifi at the local coffee shop) and updates my RSS feeds, downloads a bunch of emails based on some filters I threw together, uploads some files to my home server, and downloads some files from the same server. Then it disconnects from the wifi network, and broadcasts it's own access point until I reboot it. The Pi no longer has an internet connection at that point, but I can connect to it from the omnibook (more on that later) and grab the RSS feed or emails, or files that I marked to download, or I can drop files in for upload. 

** Backups ** - I have a script that will upload backups to my pi0w, which it will push to my server at next reboot. It's not perfect, but it works for now. 

** Questions ** - I wrote a quarter page FAQ, printed a bunch of them on my dot-matrix printer, and shoved them in my bag. When people stand expectantly at my table, motioning for me to remove my headphones, I hand them a copy. That's normally enough! Some of them even sign up for my newsletter. 

### Upcoming Solutions:

** No sound card ** - This ... I mean, it bothers me sometimes, but I mostly keep another music playing device on me so it's whatever. I recently got an OPL3LPT, and I have a music player for DOS which makes use of it. I mostly don't carry it with me because that's not what this box is for, but I have a way to use it to play music if I really want to, and that's enough. 

** No networking to speak of ** - So this isn't really fair. I have a Guru Modem, and a couple of other ESP8266 based "wifi modem" devices, and most of them work on this machine without any issues. I have to power them from an external power source, which is kind of a pain in the ass, but I can connect to BBSs and telnet to my Raspberry Pi 0w, and technically it is networking. 

But it's such a fragile solution, and I need a better one.

** Removable storage is limited to very small cards ** - The guru modem has a microSD card slot, and will allow me to transfer files on to and off of it with xmodem commands. My Pi0 has a 128GB microSD card in it. I have a couple of spare CF cards in my bag, and a CF reader for my phone. 

I also have a CD-RW drive that I can access from this box. It is Huge, and only works over parallel, so it's pretty slow. It sits on my desk near my Dot Matrix printer. If I'm using this box at home, it works. I mostly don't use this box at home, so utility is limited. 

** Useful and Interesting software for Windows 3.1 and DOS is getting hard and hard to find ** - This is a huge problem. I'm doing my part to mitigate it by writing about the software that I use, to provide mirrors of that software, and (eventually) to write new software for DOS, but this is a drop in the bucket compared to the stuff that is just Missing. 

** No TLS or working SSH ** - This is the reason that I say there's not really any networking to speak of. Have you tried to use the web without TLS today? It's almost impossible. There are hardly any DOS web browsers with SSL, and none that I'm aware of with TLS. There are two SSH clients, but neither of them support modern encryption methods. 

I have a couple of silly (and some not so silly) ideas about how to fix this. One option would be to take SSH2DOS and backport new encryption schemes in to it. This is probably the correct solution. 

The two things I'm most likely to attempt: 1) replace my ESP8266 based wifi modem with a raspberry pi 0w and a serial cable. Spawn a getty on the serial port of the pi, and log in to it as if it was a dialup shell account. I could also have it serve internet over serial via SLIRP, and even configure it to act as an SSL/TLS/JS/CSS stripping proxy. 

That would give me better solutions for backups, and real time internet, etc. It would be an excellent solution for making the Omnibook act like a modern computer (but I'm not certain that's what I want.) 

2) configure a pi or my phone to provide a torsox proxy that my guru modem will connect to, and telnet over tor to an onion address running on a home machine. Because I'm connecting to a hidden service (and there is no exit node, as a result) this is E2E encrypted. It's just ... kind of ridiculous, and still adds more hardware and more complexity to my set up. 

It also still runs the risk of making the omnibook act too much like a modern computer. 

### Other considerations

I like the idea of having some kind of networking available for the Omnibook, but it isn't actually strictly necessary. I want to be able to do the following with it: 

- write
- code
- read and respond to emails
- read and respond to fediverse posts 
- read RSS feeds
- write blog posts 
- consult reference sources 
- request data to be collected 

Technically, I could do all of those things with removable storage and some scripts running on another computer! My existing Raspberry Pi solution could be updated to act on files from a Compact Flash card connected over USB, rather than files transmitted via ftp and commands issued via telnet. 

It's entirely possible that the best solution for this problem will be to embrace the fully asynchronous nature of the way I currently interact with the omnibook, rather than trying to get *just a little* synchronous/real time networking in to my set-up. 

That being said, my goal is to have a mostly asynchronous workflow *that doesn't prevent me from doing any of the things I need to do* and sometimes the thing I need to do is to interact with other humans in something close to real time, so something *just a little* synchronous is probably in the cards.

## Next Steps

I'm overhauling my raspberry pi comms box this week. I'll do a writeup of where I land with it and take some pictures for a pst sometime before the end of the month.
