---
layout: post
category: post
published: true
title: 'A Hi-Fi Digital Audio Player for Your Home Stereo '
---
I am building a home stereo digital media player. Specifically, a small, sleek box with two wires coming out of it that I can sit next to my turntable, and plug in to my amp. It will have wifi, and will work as a dlna/UPnP receiver, so that I can cast music to it from my media server using my phone, a laptop, a desktop, or a tablet.

This is a weekend project. I do weekend projects so that I get myself out of bed on the Saturday mornings that my S/O works. This one is one of those projects that I pick up and fiddle with for a few hours, and then leave for months and don't touch because of a dumb problem that I'm unwilling to compromise on.


## Important considerations: 

- It must look like a polished, finished product, while retaining some bespoke characteristics. 
- The audio quality must be as good or better than I would get from using a Bluetooth receiver or the headphone jack on my kindle fire. (This is a low bar to clear.) 
- Ideally no or very few buttons on the finished device. 
- Must feel fun to use more often than it's frustrating. Should feel like magic if possible.


## Hardware

I'm going to do this with a Raspberry Pi or similar. Unfortunately, the Raspberry Pi 0 and the Pi 0 W do not have analog audio outputs, and the analog audio outputs on the Pi 2 and 3 are noisy. That has derailed this projects twice already. 

Now, a normal person would probably just buy an audio HAT for the Pi (I think they're ~$30), but I decided against this for various reasons: 

- I don't want to order a Hat and wait for it to arrive because this is very much a spare time project and by the time it gets here, I won't have any spare time left
- A lot of the well reviewed audio Hats aren't compatible with the current raspberry pis, or weren't last time I looked 
- I don't trust myself to solder headers on to a pi zero.
- My previous experiences with Raspberry Pi Add-on boards has been pretty subpar, leaving me less than eager to seriously consider this solution at this time. 
- (Lets be honest, I'll go that route eventually, but for now I don't have to. I'll explain.) 

Shortly after I shelved this project the last time, I started having problems with my (old, analog, tube) amplifier. I finally bit the bullet and got a mid-level Sherwood receiver. It has a (very) different sound signature than the old Stromberg Carlson radio tube based monstrosity I was using before, and it's not without faults, but I like it pretty well. 

Importantly, it has one feature that my Stromboli baby couldn't compete with: HDMI ports. It's supposed to be a home theater receiver, so it does HDMI in and out for video and audio. 

I'm planning on running this Pi headless and I don't currently have anything connected to the HDMI output of the reciever. This means that I can ignore the video, and use the Pi's HDMI audio output. No need to worry about getting a good analog out. 

It's not an ideal solution, but it's less complicated than buying a hat and running custom firmware and generally dealing with the raspberry pi addon ecosystem which (while I love everything about it, conceptually) is kind of not fun to deal with. 

**That is to say, in this case, audio over HDMI should "just work" without much intervention from me.**

## Software

Okay, that's hardware out of the way. That leaves me with two big things left to figure out: Software, Physical design. We'll start with Software. 

My gut instinct tells me that I'll be least unhappy with [RasPlex](http://www.rasplex.com). It should be easy *enough* to use, although not exactly easy. It will allow me to use my phone/laptop/tablet/whatever as a remote control for the Pi, while streaming from my home media sever. (That is to say I'll keep the music on a computer in my data closet, or on a remote server, and play it through my media player, using a third device as the UI.) 

I will likely try this, as a proof of concept, in the coming days. Importantly, I fully expect that this will **Not** feel like Magic. How far away from Magical it is will entirely determine if I stick with Rasplex. (That is to say, will it be Good Enough? I'm a big fan of Good Enough.) 

The venerable [DJ Sundog](https://toot-lab.reclaim.technology/@djsundog) suggested that I take a look at [Squeezebox](https://opensource.com/article/17/5/squeeze-pi-audio) as well. So, if Rasplex proves to be unwiedly, or generally frustrating, it will be my next stop. 

If all else fails, I'm fairly certain I could rig up something adjacent to what I want using network shares, MPD, and an android app hacked together in [LiveCode](https://livecode.org/) to serve as the controller (but, if it comes to that, this project will have to go back on the shelf for another few months until I have more than a weekend to give it.) 

## Design 

If Rasplex proves to be a Good Enough solution, my next step is to start working on a custom case. This is one area in which I am more hesitant to compromise. I'm going to have to look at this thing *all the time*, and if it doesn't look like it belongs, I'm going to disconnect it and repurpose the hardware. 

There are some Off-the-shelf cases for the Pis that come close to Good Enough. I used one for the first iteration of my [Game Console](https://www.instagram.com/p/-7ImFwn8Ew/?taken-by=analogrevolution) (we'll get back to that one soon! Version 3 is scheduled for January 2018), but this is a different kind of animal. The Off-the-shelf cases that are available are designed to be ignored. They are utilitarian, and border on ugly (which is not to say that they *are* ugly, but they get pretty close.) They're boring. That's not what I want. 

When we were running Analog Revolution, Ryan over-under-engineered some wooden cases for our custom pre-amps. They were dark stained wood, with an aluminum frontpiece. (We also put a pre-amp in [this Mott The Hoople 8-track](https://www.instagram.com/p/nicl_dn8Cz/?taken-by=analogrevolution) if I'm not mistaken. But that's a story for another day.) Something in that classical 70s aluminum and woodgrain style wouldn't feel out of place on my console, but Ryan was always the handy one, and I won't have him around for a while yet. 

The upshot of all this is that I'm going to have to get creative on the design for the case! I'm pretty excited, because I'm *good* at this kind of thing, and I don't get to flex those muscles nearly often enough. For this round, I'm probably going to go digging at the local thrift stores for something I can repurpose. 

I'll follow up with another post when I have more to report. 

(Also, obligitory link to [my Mastodon profile](https://retro.social/@ajroach42). Come tell me what you think.)
