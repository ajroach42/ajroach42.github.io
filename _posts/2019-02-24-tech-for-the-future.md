---
layout: post
category: post
published: true
title: Tech for the future
---
I'm thinking about EME and net noot and the new EU copyright directive again. And, as I always do when I get off on this topic, I'm thinking about technical solutions in addition to legal ones. Specifically, I'm thinking about technical means of fighting back against DRM, user tracking, and censorship as well as the kind of networked world I want to live in. 

I'm thinking about peer-to-peer technologies. I'm thinking about intranets and mesh networking. I'm thinking about encryption. I'm thinking about usenet, and BBSs. 

[It's the same things I always think about when this stuff comes up](http://ajroach42.com/a-modern-bbs/). 

# Software that's on my mind

These are the technologies that are currently on my mind. Some of them are the things I always come back to, some are new to me: 

## Deltachat/Autocrypt: 

End-to-end encrypted emails with multi-device support, via autocrypt, presented as instant messages via https://delta.chat. Works everywhere email works (which means intranets, traditional internet, dialup/point-to-point connections, mainframes and tildes, etc. etc. etc.) 

## Dat/Beaker: 

a neat, though unfortunately node.js\electron based system to create peer-to-peer websites using mutable torrents. I've written about [my experiments with Dat and Beaker](http://ajroach42.com/steps-towards-a-web-without-the-internet/) before. 

Dat works over an intranet or over the traditional internet. If it was a little less resource hungry, didn't run in electron, worked on low power and mobile devices, and didn't actively encourage liberal use of client side scripting, I'd probably be deploying everything via dat. As is, I'm still pretty convinced of dat/beaker as a huge step in the right direction. 

## SSB: 

[Secure Scuttlebutt](https://www.scuttlebutt.nz/) is a decentralized platform for sharing data over the internet and over LANs. It shows a lot of promise, and much of Dat/Beaker was inspired by SSB, but they work differently. I haven't spent enough time exploring SSB yet, and I'm concerned about it for the same reasons I'm concerned about Dat/Beaker

## Unison: 

"Unison is a file-synchronization tool for OSX, Unix, and Windows. It allows two replicas of a collection of files and directories to be stored on different hosts (or different disks on the same host), modified separately, and then brought up to date by propagating the changes in each replica to the other." 

## UUCP/NNTP: 

The original and the current protocols that powered usenet 

## Usenet: 

a federated system of message boards that started in 1980 and sorta still exists, but needs to be revisited/reinvinted 

## BBS/Fidonet: 

BBSs were/are message boards that ran on individual computers as early as 1978. Original BBSs supported direct dialup connections, over regular phone lines, existing outside the internet (and before the internet existed!) Modern BBSs are mostly accessed over telnet or SSH. Fidonet (and synchronet and maybe others) was a system through which BBSs called one another (or made direct connections over the internet) to share posts and emails from system to system 

## Gopher: 

the web before the web. Gopher was essentially an extension of FTP that let people present a menu based structure for accessing content on their servers and links to other servers. The Gopher protocol is much simpler than HTTP, which replaced it. Gopher can run on much lower resource machines, with implementations available for lots of operating systems including Acorn RISC OS, Amiga OS, Mac System 6 and 7, DOS, Atari TOS, NeXT, OS/2, Windows 3, Windows 9x, and most unixes. There are even gopher clients for the Commodore 64 and other 8-bit machines (though I can't comment on how well they work, yet.) 

I feel like I'm not really selling Gopher well here. Go read [what I wrote about gopher before](http://ajroach42.com/gopher-remembering-the-web-that-wasn-t/), if you want. 

## Telnet/SSH/serial terminals & mainframes/tilde sites: 

"Telnet is a protocol used on the Internet or local area network to provide a bidirectional interactive text-oriented communication facility using a virtual terminal connection." 

"Secure Shell (SSH) is a cryptographic network protocol for operating network services securely over an unsecured network. Typical applications include remote command-line login and remote command execution, but any network service can be secured with SSH." 

Both Telnet and SSH in it's basic form essentially emulate a serial cable to provide terminal access to a computer. The same thing can be done via a wired serial connection to a "mainframe" or host computer. In the 70s and 80s, this is how most non-home computers worked. Now, it's how tilde servers work (via SSH) and how most BBSs work (via telnet). There's no reason why these things need to be done over the internet instead of over a LAN. 

(I run a tilde style mainframe in my house, with local email and chat. It controls our home stereo, and can be used to play videos on one of our TVs. There's a message board, local weather reports, some home automation stuff, etc. etc. It's not connected to the internet, but once every few hours another computer that is connected to the internet connects to it, and does a little bidirectional sync.)

SSH, of course, can be used to secure more than just a command line login. Folks have speculated about using SSH as a way to encrypt gopher communications, or to build tunnels between computers for things like unison or rsync to sync files over the internet. 

## Torrents: 

Torrents are a way to share a group of files among a group of peers (with or without the internet!), but torrents (and beaker/dat) provide no encryption or anonymity, but you already knew that. 

## TOR/OnionShare: 

TOR is an overlay network that sits on top of the internet and helps protect the identity of tor users. Onionshare is a tool that uses Tor to let users securely and anonymously send or recieve files of any size.

## DNS 

The Domain Name System is the way websites get their URLs. I had largely ignored DNS until recently, but the more I think about it now, the more I don't like it. Or, rather, I don't like the idea of [authoritative name servers](https://en.wikipedia.org/wiki/Name_server#Authoritative_name_server). Unfortunately, the only alternatives seem to be: running your own nameservers, using hashes (like Dat or Tor), or just using IP addresses. None of these things feel like viable, long term solutions either. 

I don't know what the answer is, but I do know there's a problem. 

## TLS/HTTPS

HTTPS is HTTP over TLS. [Wikipedia will explain HTTPS better than I will](https://en.wikipedia.org/wiki/HTTPS). This is the foundation of modern web security. It requires us to rely on certificate authorities, and only works as far as those certificate authorities can be trusted. At the moment, it remains to be seen if this will be an effective form of general security, but it is at the very least a point of centralization in the modern internet, giving us a point of failure for security (and therefore a target for bad actors.) 

# What I'm doing 

With all of these technologies swirling around in my head, I feel like I'm on the edge of a cliff. Like I can see the outline of a future solution, but the pieces just aren't coming together for me. 

For now, I'm focussing my experiments on Beaker and Dat, and I've recently started playing with unison, a couple of flashdrives + two mainframe style offline boxes with basic web and gopher servers, as well as unison as a delivery mechanism for emails (secured with autocrypt.) 

I have a decently sized film and TV library available on peertube, and I'm going to mirror that to Dat/Beaker over the next few days. Maybe, eventually, I'll even figure out if the offline Dat/Beaker project I've tinkered with will actually work, and get instructions published for that. 

I don't know what the future will hold. I don't know if there is a way to press reset on our modern, censored, survieled internet, and get us back to something a little more local, personal, and user centric. I hope that there is, and I hope that I can help find it. For another [vision of the low-tech internet of the future, check out this article from low-tech magazine](https://solar.lowtechmagazine.com/2015/10/how-to-build-a-low-tech-internet.html). 

I'd love to hear your thoughts.
