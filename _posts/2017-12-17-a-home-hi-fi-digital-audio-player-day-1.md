---
layout: post
category: post
published: true
title: A Home Hi-Fi Digital Audio Player - Day 1
---
Over the last few days I've talked about setting up a digital home audio player (see [my initial post](http://ajroach42.com/a-hi-fi-digital-audio-player-for-your-home-stereo/), and [an update with some setbacks](http://ajroach42.com/a-quick-update-on-my-hi-fi-home-dap/).) Early this morning, I finally got the first iteration of this project set up and connected to my home stereo. After using it for a few hours, I have some first impressions to share. 

## Setup

Setup for this model was super simple and quick. I used entirely off the shelf hardware and software. 

- A Raspberry Pi Model 3 with wifi and bluetooth 
- [Rasplex media center](http://www.rasplex.com/) (an open source project, based on Kodi, but with some extra Plex specific features) 
- A [Raspberry Pi compatible analog A/V cable](https://www.adafruit.com/product/2881)

That's it! There's no fancy magic, or hidden secrets here. I'm running a wifi enabled Pi with off-the-shelf software and a commonly available cable. (A quick note on the cable: If you've never used the analog output of a Raspberry Pi before, be aware that there is no 'universal standard' for this kind of cable. Here's a good [primer on TRRS cable pinouts and the Pi](https://www.raspberrypi-spy.co.uk/2014/07/raspberry-pi-model-b-3-5mm-audiovideo-jack/).) 

### Installing Rasplex

Seriously, installing rasplex could not be easier. Download the installer for your platform, select what kind of Pi you have (Either 1 for the first few models, up to the B+, or 2 for the later models including the 2 and the 3), plug in your SD card, and press install. It took about ten minutes, and all of that was idle time. 

Then swap that SD card in to your Pi and hook it up to a monitor and keyboard so that you can link it to your plex account, and turn on Analog Audio out. 

Setting up your Plex account is handled through a setup menu, and just takes a few seconds. Once done, it will see all the libraries your account has access to, and can be controlled from the plex web app (or from a local UPnP remote.) 

Configuring analog audio out is handled from the "Preferences" screen. Of course, there are all manner of items you can configure here, but those are the important bits. Once these things are taken care of, you can shut down the Pi, detach the monitor and the keyboard, and move it over to your stereo. 

## Using the player

I use the Plex app for iOS and Android as a remote control for my headless rasplex installation. That means I can browse for music to play from my phone or tablet, and play it back on my stereo. Considering that this was the goal, I'd say that so far we are successful! 

### Interface 

The iOS and Android apps make decent remotes. If I wasn't using RasPlex headless, they would also allow me to navigate the visual interface as if I was using a more traditional remote control. This worked very well in my tests yesterday. 

As I am using RasPlex without a monitor, I can't use the traditional style remote anymore. That means that I am navigating an interface something like this: 

![screenshot (7).jpeg]({{site.baseurl}}/images/screenshot (7).jpeg)

I get to that interface from a web browser, or from a dedicated mobile app. Changes are reflected almost imediately. (Seriously, it's smoother than the BT playback in my car.) 

Playback is pretty responsive, and so far has been pleasant and easy to understand more often than it has been frustrating or buggy. (Which is not to say that it's never frustrating or buggy. Those moments still happen, but they don't happen often.) 

By and large, this setup works well! Occasionally, I still find myself noticing small ways that RasPlex excepts that you'll have a monitor connected (the initial configuration is a great example of this, but far from the only one) but in the several hours I've used it today, I have never been made to feel like this setup was hacky or impractical.

### Sound Quality 

With the cable I am using I get no interference, and I am not hearing any bleed from the video signal. So far, I also have not noticed any noise from the power supply. The DAC in the Pi still leaves a little to be desired, but it is better than on previous models, and better than I expected! 

For most listeners, I would imagine that this setup is at or above their standards for sound quality. It's close enough for me that I might not invest any effort to improve it. (That is to say, I feel like this may be the tipping point for diminishing returns. Any imptoivements that I could make from this point would probably require more effort than they are worth.) 

So, I'm going to rank the sound quality firmly in *acceptable* territory. It's not going to impress audiophiles, or win hi-fi awards, but compared to what I would have gotten out of a bluetooth reciever it is practically magical. 

## Final Thoughts 

I'm pretty happy with the whole thing. 

Visually, it's suprisingly invisble. That is to say, my Raspberry Pi fell down behind my stereo console while I was hooking up all the cables, and I left it there. I expected to have a small box to have to stare at, but as I never actually need to interact with the box, there's no need for it to be visible. 

**If we consider automotive bluetooth as our standard to clear, this setup beats every wireless car stereo I've ever used in terms of Sound Quality, Ease of Use, and Responsiveness.** 

The Interface and the Sound Quality are both good enough that I'm not actively searching for alternatives. I could be happy with this setup indefinitely.

I'm calling that a win! 