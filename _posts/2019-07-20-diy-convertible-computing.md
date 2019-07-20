---
layout: post
category: post
published: true
title: DIY convertible computing
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
- A USB hub, mouse, keyboard, and monitor (for desktop mode) 
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

A Pi 0W with SD card, power supply, case, and the requisite adapters will cost around $30, assuming you have access to a Microcenter or another source for low cost components. 

*Raspberry Pi 4* The Pi 4 is new and fancy! It's much, much faster than previous models, and supports dual monitors and up to 4k resolutions. There's wifi, bluetooth, USB 3, and much faster ethernet. The base model is $35, but it's available in more expensive packages that include more RAM. In order to support dual monitors, the Pi 4 makes a similar concession to the Pi 0, it uses a much smaller HDMI port (in this case, even smaller than on the 0) meaning you'll need a special cable or an adapter to use it with a standard monitor. 

Additionally, and importantly, the 4 is reported to run pretty hot, with the official guidelines calling for at least a heatsink, and many people suggesting that active cooling may be needed. 

A Pi 4 with SD card, power supply, case, and video adapter will cost around $55 on the low end. 


*Raspberry Pi 3+ and other pi models* The Pi 3+ is my personal choice for projects like this. They also have an MSRP of $35, but are frequently available for less (at least, in my area.) They have built in wifi and bluetooth. They run a little hot, and need a little more power than a 0, but not as hot or as hungry as a 4. Importantly, they have a full sized HDMI port, and 4 full sized USB 2 ports, and do not require adapters. 

A Pi 3 with SD card, power supply, and case can be had for around $45. 


### Battery 

There are several options for powering a pi on the go. They fall in to, broadly, three categories. 1) basic cellphone backup batteries, 2) nice cellphone backup batteries, 3) internal batteries + power boost circuits. I'm not going to spill many bits here: 

- Basic batteries don't have charge pass through, so you can't charge the battery while it is powering the device, and you must shut it down before switching from wall power to battery power or vice versa. This is a bad option. It is much more of a hassle than it sounds like it would be, and it already sounds like a hassle. Don't do this to yourself. 

- Nice batteries do have charge pass through, so you can charge the battery while it is powering the device, and you can plug in/un-plug the battery without shutting down the device. Many devices that offer this don't advertise it, so it can be hard to find a reasonably priced battery with pass through. This is generally the best option. 

- Internal batteries are what it says on the tin. You get something like a [Power Boost](https://learn.adafruit.com/adafruit-powerboost-1000c-load-share-usb-charge-boost/overview) and hook up a battery to it. The power boost up converts the voltage from the battery to match what the Pi needs and handles charge pass through. If you're doing anything other than a fully modular design, I recommend seriously considering  this route, but it does add cost and complexity (the charge circuit alone is usually $20. Paying $20 for the power boost plus another $30 for the battery seems kind of silly if you're going to connect it to a $5 computer.) 

### Monitor 

There are Many monitors, but they broadly fall in to four categories: High-res HDMI, Low-res HDMI, Composite, SPI. Unless you have a good reason to, don't bother with composite monitors or SPI monitors. The first is *very* low res and often full of chromatic aberations, the second updates the screen pretty slowly. The benefits of both are entirely lost when working on a fully modular design. 

As for the HDMI options, they are available in sizes from 5" up to 11", and resolutions from from 800x480 up to a full 1080p. They vary in cost depending on where you buy, and who manufactured the display, but I would expect to pay between $40 and $80 for a good monitor without touch at any size under 10 inches, and double that for one above inches. These can usually be powered from the USB port on the pi directly. I'm a fan of Adafruits HDMI4PI line, but there are other cheaper options available as well. 

Resistive and capacitive touch screen models are also available, but I wouldn't bother with one of those for this use case. 

### To sum up: 

- A Single Board (SoC) computer ($10 - $50) 
- A case for the computer ($5 - $10) 
- One or more power supplies ($5 - $10 each) 
- A USB hub, mouse, keyboard, and monitor (for desktop mode) *I am working under the assumption that you already have these, or will be acquiring them seperately, and will only be discussing the portable operation. This stuff is expensive* 
- Adapters (if needed) (up to $15) 
- A smaller keyboard ($10 +) 
- A monitor (for portable mode) ($40 - $80) 
- A battery (preferably one with pass through charging) ($30+)
- Storage (If you're using a raspberry pi or similar, this will likely be a microSD card) ($5 or less from microcenter)  
- Some kind of rig to hold all the portable bits (up to you) 

for a base price of $105 - $245 


## Fully Portable 

I first saw this [a few years ago](http://ajroach42.com/the-zero-terminal-a-handheld-raspberry-pi/) [from n-o-d-e](https://n-o-d-e.net/zeroterminal.html). The basic idea is to stick a Pi 0W, a battery with a charge circuit, and [a PiTFT Plus 480x320](https://www.adafruit.com/product/2441) in to a sliding BT keyboard phone case. 

The end result is surprisingly slick and usable. I built one of my own shortly after seeing this article, although I sadly don't have any pictures of it, and I've long since deconstructed it for parts. I don't love the SPI screen, but it makes for a really slick finished product that is actually pretty fun to use. 

I didn't have a 3D printer when I built mine, so I encased the top in some scrap cardboard and some duct tape. It worked well enough, and I carried it with me for a few weeks, before realizing that it met the needs I had in previous years when I was working as a web developer, but it did not meet my needs at the time. 

iPhone 5 keyboard cases are hard to find these days, but any sliding BT keyboard case will do, and they can be found for less than $20 all day. 

Total for this model: $120 (including the USB and HDMI adapters you'll need for desktop operation.)  

## Tablet Style 

This is probably the most appealing method on first glance, and I've toyed with it on more than one occasion, but I've been consistently disappointed with the results, mostly on a software level. The basics: A pi with the needed bits ($30 - $55) an [official RasPi foundation touch screen](https://www.adafruit.com/product/2718)($80) and a case (several options, $10+). You add to that a wireless keyboard, and that's it! 

Of course, you'll probably want a battery too. See Batteries in the modular section for thoughts on that, and add it to your $120.

You end up with a weirdly thick and kind of fragile tablet running at 800x480 with a pretty nice capacitive touch screen. 

Depending on what software you end up using on it, this actually works pretty well. I used a cellphone backup battery with charging pass through and 3D printed a little stand for the touch screen that ended up looking something like an Apple IIc. In practice, though, I found that 800 x 480 was too low of a resolution to use for most graphical applications, and that I could get a better non-touch monitor for a text terminal for the same amount of money, so that's the route I'm going next. 


## In practice 

The Pi line, through the pi 3 at least, is not powerful enough for a modern desktop and web browser. If you want to run a CLI/TUI environemnt, it'll do just fine. If you're willing to go for lighter desktop apps, it can be very snappy. If you want to watch youtube, expect to wait often. 

The Pi 4, I've been told, can deliver a full desktop experience. I'll find out if that's true soon. 

For my modular pi rig (which features a pi0, backup battery with charging pass through, and a 10" HDMI monitor clamped to a mechanical keyboard) I mostly use it to access other machines on my network over SSH, or to access email (via Mutt) and a text editor, when real computers get to be overwhelming. I've used it with omxplayer to watch videos and cmus for music. I've used it as a mobile server and LAN, I've used it as a serial gateway for my vintage computers. 

It does what it's told, always. Sometimes, it's just a little slow. 

I've used a pi3 as a full desktop in the past, and as long as you don't place too many demands the web browser, it'll do the job. (Heck, it'll even play youtube, eventually.)
