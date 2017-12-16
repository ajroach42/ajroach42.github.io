---
layout: post
category: post
published: true
title: A Quick Update on my Hi-Fi Home DAP
---
I spent a few hours today putting together a proof of concept Digital Audio Player based on [RasPlex](http://www.rasplex.com) as discussed in [yesterday's post](http://ajroach42.com/a-hi-fi-digital-audio-player-for-your-home-stereo/). I had some Successes and some Failures that I'd like to discuss here. 

## First, the bad news:

My reciever does have HDMI inputs, and it does do digital to analog audio conversion, but those things are separate. That is to say, the HDMI inputs are Pass-through only, and do not get decoded. This means that my dream of using the HDMI output of the raspberry pi to connect to my home stereo will not be a reality without a newer reciever. 

Apparently, this is pretty common for entry level and mid range A/V recievers. It sounds completely daft to me, but I've stayed away from video technology, so I don't know the technical reasons behind this. As a result of this bizarre design decision, I wasn't able to use this as a solution for my needs but, *if your reciever supports audio playback over HDMI, Rasplex and a Raspberry Pi 3 could make an excellent Digital Audio Player.*

## Now, the good news: 

I wasn't able to use the device the way I wanted to, which is a real bummer. But! I did get to spend a few hours playing with RasPlex, with the device connected to my TV. RasPlex works really well! The controls are slick, and pairing it with my Plex account and media servers was a snap. The Plex app for iOS and Android makes a great remote, and I was also able to make use of a UPnP app to control it. 

RasPlex, at least in my limited experience with it today, was also more responsive, and easier to use than the Plex app for Roku. The UI was quick and responsive, playback was smooth. 

Of course, it doesn't matter how quick the UI is if we're going to run it headless, but I haven't had the chance to try that yet. 

## Next Steps

For now, my plan is to get an an Analog A/V cable for the Pi and configure RasPlex to use that for audio output. I'm generally not a fan of the Pi's onboard DAC, and I've found the output to be pretty noisy, but I've only ever used it with a TRS -> RCA cable, instead of the TRRS -> RCA cable that the Pi is supposed to use. It is my hope that using a well insulated cable, with the video signal actually isolated on it's own ring of the connector will reduce some of the noisieness. 

Then, I'll live with the thing for a few weeks, and make a decision as it if this software works well enough, and is pleasant enough to use, to merit further improvements.
