---
layout: post
category: post
title: I Launched a Cable Network
published: false
---
[I launched a Cable Network](https://newellijay.tv/2024/10/26/new-ellijay-television-now-on-cable/). If you're in the Ellijay Telephone Company coverage area, you can watch it on channel 176. If you're not, you can [watch it online](https://vod.newellijay.tv/w/hPrMTPpUuP8ZLoaqHTkLmd) or on [roku](https://channelstore.roku.com/details/923c7927ca06324871b965f166805a5b/new-ellijay-tv) (or even embedded on this post!) The whole thing is a Community Centered, local first production and broadcast, powered entirely by free software. Click through to watch the stream and learn more about how and why I built it. ![New Ellijay Television now broadcasting on ETC channel 176, online and on roku!]({{site.baseurl}}/images/Untitled-design57.png)


<iframe title="ON AIR" width="560" height="315" src="https://vod.newellijay.tv/videos/embed/883211f7-723a-4ecd-b2fd-7a4ad1e3d70c" frameborder="0" allowfullscreen="" sandbox="allow-same-origin allow-scripts allow-popups allow-forms"></iframe>


## How 

If you've ever wondered if it's possible to run a broadcast television network on commodity hardware using open source software when you have no idea what you're doing, the answer is absolutely yes. I'm doing it right now. We're streaming out to Cable, to a roku app, and to the web. 

Under the hood, we're using the following software: 

- Peertube
- A fork of the PeerVue roku channel 
- [ffplayout](https://ffplayout.github.io/) 
- ffmpeg 
- and for production, we lean on kdenlive and ardor. 

That's pretty much it. You string those pieces up in the right order, and you can have a streaming service and a VOD platform. If you're in the US, and you call your cable company and pay them their Leased Access fees and add an "impulse decoder" to the mix, you can be on cable. 

### Distribution Pipeline

We're running ffplayout on the server side, building our schedules by hand (new open source scheduler and media asset manager coming Soon ™️) and outputting to SRT and RTMP. 

The RTMP stream is consumed by peertube, and then spit back out to our roku channel. The SRT stream is consumed by a piece of hardware at the cable company (an Impulse 300D Network Decoder) which takes the SRT stream and just shoves it in to their head end. 

The Impulse Decoder is the only piece of equipment in all of this that isn't a computer running debian or a cheap rented VPS (also running debian,) and whatever it's running is the only time any of these videos touch something that isn't free software. (It was also the least flexible part of the setup, and for several weeks the bane of my existance! But that's neither here nor there.)

We manually build a playlist in ffplayout, ffplayout builds our SRT stream for the cable company (which then [gets re-encoded by another ffmpeg process](https://retro.social/@ajroach42/113278866789695300) to smooth over the problems that the Impulse Decoder had when we first started broadcasting, but again that's not super important) and then, from the same playlist but in a separate process, ffplayout builds our RTMP stream for peertube. 

Peertube powers our online livestream as seen on our website, and our roku channel as well as our Video On Demand. (When I finish my DIY cable box project, peertube will also power that.)

### Production Pipeline 

The vast majority of our videos are captured on second hand 10+ year old cameras. There are a few newer cameras in the mix, but they're significantly less common and frankly less useful. Using old cameras is fine! They look fine! They shoot in HD, and we're broadcasting in SD (well, our live stream goes out at 720p, but the cable broadcast is SD) so it doesn't really matter. 

Any camera from the last decade is going to look a whole world better than the best television cameras of the 80s and 90s. Even our cheapest digital cameras (we use a lot of Kodak "flip" style cameras, because they can be had for under $30 on the used market and run on AA batteries) produce footage that looks Good Enough for television. 

(And, occasionally, we'll shoot on a consumer video camera from the 60s or 70s, and get video that is unquestionably worse than Television quality, and everyone loves it!) 

We take the footage from those 10 year old cameras and we catalog it in nextcloud and it syncs to everyone who is involved in production. This is my least favorite part of the process because Nextcloud does not work very well. But it gets the job done most of the time. 

Then we edit in kdenlive. 

Audio is recorded, as needed, in ardor or audacity, and edited in the same place (or it's recorded on purpose built hardware, like old Zoom recorders, rescued from the digital landfill and edited in ardor, audacity, or directly in kdenlive.) Or it just comes from the camera. 

Most of our editing is also done on second hand/landfill rescue computers. Most of our programming is edited and rendered at 720p or lower because that makes it cheaper and easier to work with on old hardware. Broadwell/5th Gen intel hardware is more than capable of editing and rendering 720p video, and is often available for free or very cheaply (we work with an electronics recycler to get former workplace machines. There's probably one in your area!) 

The bulk of our original material is released CC-BY-SA because I believe in giving back to the commons and I think CC-BY-SA is the best currently available license to Empower creators while disincentivising exploiters. (See [The Small Things Manifesto](https://ajroach42.com/the-small-things-manifesto/) for more on licensing.) 

## Why 

I wrote a zine last year, a short book really, about why. You can [read it online](https://communitymedia.network/). I am working on a revised version that covers our broadcast cable initatives. Basically, though, the why is pretty straight forward: 

A very small number of very rich people control the vast majority of what people see online, and *even when people mostly consume independently produced content from places like youtube, twitch, or tiktok* their feed is generated by a corporation that values engagement, attention, and the accumulation of capital over the well being of the viewer. 

I've been writing about this for over a decade. In 2017, I published [this piece entitled DIY MEDIA](https://ajroach42.com/diy-media/) which was adapted from an article in a zine I originally published in 2014. It bangs the same drum. 

In 2022 I published [The Small Things Manifesto](https://ajroach42.com/the-small-things-manifesto/), which ultimately covers many of the same topics. 

If we want to change the world, we have to change people's minds. If we want to change people's minds, we have to replace Corporate Media. It was true with The Videofreex said it, it was true when [Shamberg called corporate TV Beast Media, and it was still true even when he said that youtube was the culmination of the original ideas of the DIY TV revolution (he was wrong.)](https://sites.evergreen.edu/mediaworks1516/wp-content/uploads/sites/121/2016/01/Merrin_2012.pdf). 

We're out here making the world a better place, and we're doing it by making [fiction about Bigfoot Hunters](https://vod.newellijay.tv/w/3h6m3uZSkBjrHYVLMA3m1o?start=0s), and [non-fiction about Pro Football](https://vod.newellijay.tv/w/cia4J3tkqgvhZrdpNL3Cps), and half a dozen things in between. 

## How can I help? 

We're looking for [direct individual sponsors](https://newellijay.tv/sponsor-us/), we're looking for [advertisers](https://newellijay.tv/advertise-with-us/), we're looking for programming to syndicate, we're looking for more viewers. Watch our programs, spread the word, give us money. All the usual. 

Reach out to video at NewEllijay dot TV if you'd like to learn more about our advertising program. Packages start at $225/month, with up to 3 months free under some circumstances. 

Thanks!
