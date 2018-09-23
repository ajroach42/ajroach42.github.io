---
layout: post
category: post
published: true
title: Social Networking for the 90s.
---

As I mentioned in a recent post, I have started using a Gateway Handbook 486 as part of my daily workflow. It's a little DOS laptop that you can read more about in [my previous post](http://ajroach42.com/blogging-at-19200-baud/). One of my favorite things about using this machine has been Social Media. This post is about how I'm interacting with Social Media and Blogs from a DOS laptop, and how you can apply the same techniques to your life for fun and profit.

First, let me make something clear on the front end, I am cheating. I am using the Handbook as little more than a display and keyboard for at attached Raspberry Pi. On the one hand, this means that these methods will change and evolve as I improve my DOS networking setup, on the other hand this means that every technique, tool, and idea I'm using here is equally applicable to any Linux, Mac, or Android computer (and even Windows 10 with Cygwin or WSL.) 

Now that my warning is out of the way, let's talk about what it's like to use the modern, social web from a serial terminal. 

## Links

Links is my CLI browser of choice. I've used several variants (including Links2 and Elinks), but they are similr enough on the surface, and in their user interface, that they are essentially interchangable for our purposes. 

There are text mode browsers, with decent UIs, and support for some modern conventions like tabs. They don't render Javascript, and barely render CSS, which means that they are *fast* and *ugly*, and lots of things are broken. 

So many thing are broken, in fact, that it is difficult to use Links as your daily driver without making some changes to the way you interact with the web. In my experience, I'm happier having made these changes. 

I will swap over the lynx if I need to access a Gopher site, but most of my browsing is currently in Links. 

### Mobile sites 

Most interactive websites that have been around for at least ten years (facebook, twitter, etc.) or are popular in places where smartphones are still uncommon have a dedicated mobile site that presents a stripped down version of the service with no javascript. Facebook, Twitter, and Gmail are all perfectly usable from Links via their mobile sites. I try not to spend any time on any of these services, but if I must, I do it through their mobile sites. 

### Brutaldon 

My social media platform of choice, Mastodon, heavilly relies on Javascript. It doesn't work at all (in a browser) without JS. There are some desktop/CLI clients for interacting with Mastodon, but I've found the best way to access the Fediverse to be via [Brutaldon](https://brutaldon.online) a brutralist mastodon client that targets Lynx compatibility. It works pretty well for my needs, and can be self hosted. 

## Chat (libPurple) 

I spend a lot of my day in various IM conversations. Thankfully, Pidgin/LibPurple has a command line client in the form of Finch. Using Finch I can access FB Messenger, IRC, XMPP, etc. There are also slack plugins, but I only use Slack for work, and I only use the Handbook outside of work, so I haven't bothered with it. 

## Blogging 

I run this blog using Jeckyl, and store it in a git repository. Both of these things work better from a command line. I have access to emacs and nano and I can blog however I want. 

### Reading blogs 

Newsbeuter is an excellent RSS reader. I have recently imported all of my RSS feeds in to it, and between that and my Palm Pilot, I rarely look at the news or a blog post from anywhere else. 

## Email

Mutt is my mail client of choice, in most situations. I have it configured to check my personal emails via IMAP, which is working okay. I'll likely make some changes to this setup soon (likely in conjunction with finally getting native networking on the Handbook) 

## BBS

For now, I'm BBSing via telnet from my shell connection, but I'll be much happier when I can BBS directly from the Handbook. (Expect to hear more about BBSs in the future.)
