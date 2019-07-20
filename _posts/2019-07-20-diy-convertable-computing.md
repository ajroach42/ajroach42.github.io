---
layout: post
category: post
published: false
title: DIY convertable computing
---
This is a post about building your own Desktop/Portable computer. I'm presenting several options for classes of hardware and methods of interaction. This post is specifically about hardware, I might do another one about software. I'm also trying to meet some specific requirments (low weight, long battery life, ability to run emacs above all else, networking not needed), which means I will be making some suggestions and observations here that differ from what I might say in more general circumstances. 

Alright, now that the intro is out of the way, a friend said to me today:  

> I want a small computer that can sit at my desktop and get plugged into power and a hdmi'd to a big monitor and its wired keyboard and mouse, and then I can unplug it and use it off a battery with bluetooth keyboard and hdmi'd to a small screen.

This was at the end of a pretty long discussion about tablets and laptops and the death of the netbook before ultimately alighting on Raspberry Pi, and other DIY options. I felt like this is something other people might also like, and that it merrited some longer observations, so here we are. I see three basic methods by which this could be achieved: 1) fully modular, 2) fully portable (the [N O D E 0 terminal](https://n-o-d-e.net/zeroterminal.html) method), 3) Tablet Style. 

## Fully Modular 

The modular method is probably the easiest of the three to understand, and is the closest to the design that my friend requested. For this method you need one of each of the following components: 

- A Single Board (SoC) computer 
- A case for the computer 
- One or more power supplies 
- A USB hub, mouse, keyboard, and monitor (for desktop mode) *I am working under the assumption that you already have these, or will be acquiring them seperately, and will only be discussing the portable operation.* 
- A smaller mouse, keyboard, and monitor (for portable mode) 
- A battery (preferably one with pass through charging)
- Storage (If you're using a raspberry pi or similar, this will likely be a microSD card) 
- Some kind of rig to hold all the portable bits

The beauty of this design is that it can be completely modular. If you don't like the mouse or the keyboard or the screen, sell it and buy another. Each piece can be used on it's own. This modularity comes at the cost of portability, and possibly at the addition of weight.

There are a couple of options available for each piece of hardware mentioned above, and I won't discuss the pros and cons of every USB hub or Keyboard on the market, but I do want to spend a few cycles on the portable monitor, battery, and SoC. 

### SoC 

Depending on your budget, your region, and your needs, you might pick from dozens of single board computers from the Odroid line, the Atomic Pi, the Orange Pi, the Chip (R.I.P.) and of course, the Raspberry Pi. For the purposes of this article, I'm going to focus on The various Raspberry Pi as they are the most commonly available, and often the most well documented. Your needs will vary, and you should feel free to disregard this advice. 

*Raspberry Pi 0W* The 0w has a couple of benefits: Low power consumption, low price ($10 MSRP), small size, built in wifi and bluetooth, and low heat output. 

If you don't need the wifi and bluetooth you can also look at the 0, which can be found for as little as $5. The 0W isn't perfect, though. It's slow, and it does not have any full sized ports, requiring an adapter to connect a full sized USB or HDMI cable. These adapters are commonly available, and not terribly expensive (less than $5 each) but they do add additional complexity and cost, undercutting the low price of the 0 and making the 3 or 4 seem more attractive. 

*Raspberry Pi 4* The Pi 4 is new and fancy! It's much, much faster than previous models. 



*Raspberry Pi 3+ and other pi models*


### Battery 

### Monitor 

## Fully Portable 

## Tablet Style 

## In practice 