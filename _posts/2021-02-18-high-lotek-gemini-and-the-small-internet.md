---
layout: post
category: post
published: true
title: High Lotek - Gemini and the Small Internet
---
As was probably inevitable, I've spent the last few weeks poking around with Gemini. I want to take a few minutes to talk about what Gemini is, what it isn't, and why I care. 

## What is Gemini? 

* It's a protocol partway between gopher and the web, without tracking, with encryption by default, respectful of users above all else. 
* It's a small corner of the internet without multiple turing complete markup languages, operating on a non-capitalist, human scale.  
* It's an effort to make the internet a little more personal 

In the gemini FAQ, Solderpunk says 

> Gemini is a new (the project started in June 2019) application-level internet protocol for the distribution of arbitrary files, with some special consideration for serving a lightweight hypertext format which facilitates linking between files. You may think of Gemini as "the web, stripped right back to its essence" or as "Gopher, souped up and modernised a little", depending upon your perspective. Gemini may be of interest to people who are:

* Opposed to the web's ubiquitous user tracking
* Tired of obnoxious adverts, autoplaying videos and other misfeatures
* Interested in low-power computing and/or low-speed networks

> Gemini is intended to be simple, but not necessarily as simple as possible. Instead, the design strives to maximise its "power to weight ratio", while keeping its weight within acceptable limits. Gemini is also intended to be very privacy conscious, to be difficult to extend in the future (so that it will *stay* simple and privacy conscious), and to be compatible with a "do it yourself" computing ethos. For this last reason, Gemini is technically very familiar and conservative: it's a protocol in the traditional client-server request-response paradigm, and is built on mature, standardised technology like URIs, MIME media types, and TLS.

The FAQ is great, and you should read the whole thing. 

[Solderpunk's Gemini FAQ](gemini://gemini.circumlunar.space/docs/faq.gmi)

## What isn't Gemini? 

* A replacement for the web. 
* A replacement for Gopher. 
* The future of the internet. 

To quote solderpunk again: 

> Gemini is not intended to replace either Gopher or the web, but to co-exist peacefully alongside them as one more option which people can freely choose to use if it suits them. 

## Why do I care? 

Above I said that it was inevitible that I'd end up playing with this tool. When I say that, I mean I've been talking about the failings of the Modern Internet for a really long time. See for example:

* [Steps Towards a Web without the Internet](http://ajroach42.com/steps-towards-a-web-without-the-internet/)
* [Gopher, remembering the web that wasn't](http://ajroach42.com/gopher-remembering-the-web-that-wasn-t/)
* [Observations on the digital mistakes of our last 10 years](http://ajroach42.com/observations-on-modern-computing-the-last-10-years-were-a-misstep/) 
* [A Modern BBS](http://ajroach42.com/a-modern-bbs/)
* [Net Neutrality, The Consolidation of American Media, and you](http://ajroach42.com/net-neutrality-the-consolidation-of-american-media-and-you/)

and circa 2017 I was constantly having the same conversation online, a conversation at the time which was centered on the future of Gopher. Lots of people were talking about the ways the web had failed, and the ways it had succeeded, and what there was to be done about it. One solid proposal that kept coming up again and again was an extension to the Gopher specification. 

* [This thread on Mastodon is a good example of that conversation](https://retro.social/@ajroach42/99051400673074933) 

In that thread, I list the following goals: 

* A gopher client with the ability for the user to select fonts and colors for menus. 
* A gopher client that renders HTML, Markdown and Plaintext. 
* While rendering HTML, it explicitly ignores any scripting or styling (aside from anything the user has defined.) 
* The client offers users the option to download and render inline images in HTML and markdown files (but only over gopher) 
* Links within HTML and Markdown files to work the same as in menus.
* Security/Encryption 

(That client exists today. Several do, but the one that comes closest to what I described there is called Kristall. It's a gemini client that also supports gopher, finger, http (with only the most basic HTML), and markdown rendering and it's pretty great.) 

[The Kristall browser on github](https://github.com/MasterQ32/kristall)

In that same thread, I said: 
> Gopher is just a weird little non-capitalist, human scale way for us to publish and consume stuff. It's fun, it's easy, and it's a weird way for folks (like you and me) to resist, in our own small way, the shit that the big centralized services do, and the things that netflix pushed the w3c in to doing.

Gemini is a weird little non-capitalist, human scale way to publish and consume stuff, and it has been Fun so far. 

If you find yourself looking for a Smaller internet, or maybe for a Bigger Gopher, come give it a look. 

## Hosting

I'm using gmnisrv on a VPS, and it works reasonably well. Selfhosting is also possible on something as simple as an SBC. 

Lots of other hosting software exists, of course, and I might move to something else eventually. 

## Browsing 

I mentioned Kristal above, which I've used and enjoy a great deal. I'm also using Lagrange at the moment, and I really like some of the things that it does. 

Each is still under development, and I expect both to evolve in interesting ways. 

There are terminal clients too, but I'll look at those in another post.
