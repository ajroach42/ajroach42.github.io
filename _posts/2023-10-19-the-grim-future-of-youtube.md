---
layout: post
category: post
published: false
title: The Grim Future of Youtube
---
*The short version:* Corporate sponsored video sharing platforms are always going to disappoint you, so try something else. Today, the something else that I'm offering is [Community Media Video](https://communitymedia.video), this is paid peertube hosting with 10GB for storage for $15/year. *What follows:* a discussion of the way youtube is bad, and will likely continue to get worse.

Right now, Youtube is serving a mild rebuke to some people who try to view youtube with an adblocker, and I believe this is an ill portent of things to come. Right now, youtube warns users that ad blockers are in violation of youtube's terms of service. (I suspect that ublock origin will be blocking this pop-up within days, if it doesn't already, but that's not the point.) 

This is the first step on a road towards a much different Youtube, and it speaks of a potential future with a much less free Web. So lets explore what is likely to happen to the web in the coming months and years, and what we can do about it. 

## An aside: Use an adblocker, no matter what youtube says

Before I go down that road, you should absolutely be using an ad blocker. Try [Privacy Badger](https://privacybadger.org/) or [uBlock Origin](https://ublockorigin.com/). It's not just about blocking ads, it's about your privacy and security on the web. The internet is much more pleasant, much faster, and much safer when you aren't bombarded with advertising from every corner. 

## Chekov's Browser Standard

What I want to talk about today isn't adblockers, but rather the logical next steps from what Youtube is doing today. Based on google's track record, frankly, things are likely to get ugly. 

First we have to talk about Checkov's browser standard, [EME](https://en.wikipedia.org/wiki/Encrypted_Media_Extensions). 

Encrypted Media Extensions are a way to serve [DRM](https://www.defectivebydesign.org/what_is_drm) restricted files over the web without using a third party plugin like Flash. The introduction of EME was widely protested by a whole host of members of the w3c, but it was eventually adopted in a sketchy back room deal that laid the foundations to compromise the modern internet. 

Fun right? 

[As of 2020, it was basically impossible for any small player without major funding to implement a fully standards compliant web browser because of the fees associated with EME access.](https://boingboing.net/2020/01/08/rip-open-web-platform.html) This hasn't been a widespread disaster, yet, for several reasons, but it's likely to become one. 

EME support was slow to roll out, and only places like Netflix mandated it in the earliest days. For half a decade, it was basically impossible to watch netflix on a computer running linux (and, even today, it still occasionally requires [an ugly workaround involving the Widevine package for chromeOS](https://gist.github.com/ruario/19a28d98d29d34ec9b184c42e5f8bf29) if you're going to watch netflix on, say, a Raspberry Pi.)

Google was one of several major companies that pushed the W3C to adopt EME as a standard for web browsers, and they've [recieved](https://boingboing.net/2019/05/29/hoarding-software-freedom.html) [major](https://boingboing.net/2018/06/26/saudi-v-russia.html) [pushback](https://boingboing.net/2017/09/21/democracy-dies-in-dullness.html) (and not all of it was from Cory Doctorow, but the best bits were.)

Running an adblocker on youtub is now a violation of Youtube's terms of service. It was a commonly held theory, for years, that violating a website's terms of service was a violation of the CFAA. [Thankfully, courts have softened on that.](https://arstechnica.com/tech-policy/2020/03/court-violating-a-sites-terms-of-service-isnt-criminal-hacking/) In spite of failing to make adblocking a criminal offense, google has signaled that they may start blocking ad-blockers from accessing youtube all together. 

EME is one route they could take to do this and, in doing so, they would likely break tools like [Youtube-DL](https://github.com/yt-dlp/yt-dlp) and [Invidious](https://github.com/iv-org/invidious), both of which they've begrudgingly tollerated and fought back against in turns over the last decade. YoutubeDL is a vital tool for archivists, and invidious is an incredibly valuable privacy tool. EME would destroy them both, and bypassing EME would almost certainly be a criminal violation of the DMCA. 

This would be a big deal for several reasons: 

- Youtube consumes an inordinate amount of data about you, from all over the web, and uses it to build a detailed tracking profile which Google has a track record of mishandling. 
- Google has already killed one video service (google video), deleting countless hours of content from the web. 
- Youtube is notorious for taking whole channels off-line as the result of spurrious copyright claims
- Google has, in the last year, threatened to remove all video content uploaded by inactive accounts (they eventually backed off of this plan, but only after massive public outcry)
- Simply put, the general public treats youtube like an archive, but youtube can be incredibly temporary under the wrong circumstances. 
- With mandatory DRM for youtube content, using tools like Youtube-DL would suddenly be actual criminal violations of the DMCA, probably, I'm not a lawyer. 

Computers are good at copying things. It's probably what they're best at. But, due to a combination of rent seeking, bad legislation, and outdated copyright laws, we keep coming up with a bunch of artificial limitations on how computers can make copies of things. This is bound to be expensive, and ultimately doomed to failure, but in the meantime a lot of art and media is likely to be lost or destroyed. 

[We, as a species, are fond of that kind of thing.](https://ajroach42.com/we-are-terrible-stewards-of-history/)

I've been [writing about archiving your work for years.](https://ajroach42.com/document-your-art-how-to-archive/) It's vital to the principles of [Community Media.](https://communitymedia.network), and distributing your work under a license and through a platform that makes re-sharing possible is a vital component of archival. 

To that end, if you're looking at the likely future of youtube as a DRM encumbered distribution hub that forces you to sit through countless ads in order to watch a video your grandfather posted before he passed away, only to discover that the video is no longer available because Warner Brothers issued a copyright strike as a result of a brief snippet of a 70 year old song that can be heard briefly in the background on the radio, and you're wondering what to do instead: 

- Archive.org will let you upload videos for free, with some reasonable limitations, and they'll stay up as long as the archive exists. 
- It's possible, and even easy these days, to self host something like peertube.
- If you don't want to self host, consider signing up for an account on [Community Media ($15/year for the base package.)](https://communitymedia.video)

By all means, upload to youtube if that's where your audience lives, but don't expect it to be around forever. 
