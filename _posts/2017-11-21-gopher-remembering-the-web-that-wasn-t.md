---
layout: post
category: post
published: false
title: 'Gopher: Remembering the web that wasn''t'
---
This is an article about Gopher, a service that existed on the internet before the web. It's also an article about how the web is broken, and some speculation on how Gopher might fix that. [If you want a more general overview of Gopher, try this article from Tedium](https://tedium.co/2017/06/22/modern-day-gopher-history/). If you want a more general overview of how the web is broken, try every thinkpiece titled "The web is broken" on Medium. 

-------------

The modern web is an ugly, massive, broken mess. This isn't a secret or a new take or a controversial opinion. We stuff our webpages so full of tracking cookies and bitcoin mining advertisements and javascript apps that monitor your every move that it's no wonder that modern web browsers are less effecient than ever. Pages are huge (many MB per page, easy) and they spy on you. The average web page with advertising will send all manner data about you back to maybe a hundred different sources.

I monitored a web page the other day, and it transfered 5MB worth of data to advertisers out of my browser. Do you understand how ludicrous that is? 

5MB of data from my browser to several different servers all over the web. What information could they possibly be gleaning out of my browser to justify 5MB upload? 

Then you add to the fact that every time you load up a web page, you're literally just willy-nilly executing whatever code is in the page. Javascript and CSS are both turing complete programming languages that can be used to completely hijack your machine and skim your resources for purposes you'd never know about if you weren't paying close attention. (I wasn't kidding about ads [mining bitcoin in your browser](https://www.theguardian.com/technology/2017/sep/27/pirate-bay-showtime-ads-websites-electricity-pay-bills-cryptocurrency-bitcoin). This is costing you money, and shortening the life of your hardware.) 

I am of the opinion that the current direction of growth for the web has been a mistake. The fact that we've let the web get to the state it's in now is unforgivable and frightening. It is time for us to seriously consider how to move forward. 
 
So I've been thinking about Gopher. I really would love it if you'd read [this peice someone else wrote about the history of the Gopher protocol](https://tedium.co/2017/06/22/modern-day-gopher-history), but I'll do my best to sum it up. 

Gopher was this service that existed before the web did. It was real simple. Just menus, and files. Doesn't get any simpler than that. It's still around, if you have a webbrowser that supports Gopher (you don't, probably) or if you want to use a gopher to web proxy (you don't, probably) or if the gopher server also serves http (this is more likely, for now) or if you have a dedicated Gopher browser (more on this later) 

_tl;dr Gopher is a service that lives on the internet, but has existed longer than the web It allows people to share files on the internet, with basic links and menus, but without interpreting and executing code on your machine each time a page loaded._

I run a gopher server at gopher://ofmanytrades.com that can also be accessed from the web at http://ofmanytrades.com:70

If you click on that, you'll see how it's just menus and text. 

In the Magazines/Dungeon Magazine or Magazines/Pulps folder there are direct links to PDFs. I didn't build that page, I just put the files in a folder, and let the server build the menus. 

Or click on Music, and then on 78s. From there, you can see literally 5000+ songs from Archive.org's 78RPM collection. Click on one and listen to it. [Here's a good one, if you're overwhelmed by the 5000+ options - Muddy Waters, I don't know why.] (http://ofmanytrades.com:70/Music/78s/I%20Don%27t%20Know%20Why%20-%20Muddy%20Waters%20and%20his%20Guitar.mp3) 

Neat right? 

In the books folder there are HTML files (you know, web pages!) that can be downloaded and viewed with an HTML interpreter (you know, a web browser!) or, in many cases, viewed directly in the Gopher client. Eventually, there will be more of these on my server. 

Now, I'm sure at this point you may be asking what makes gopher better than the web, if I'm going to use it to serve up HTML pages just like a website. That's a good question! The answer is that no gopher server *requires* a web browser. You could download my HTML files and open then in [Dillo](https://www.dillo.org/) or you could use Lynx to navigate both the Gopher server and the HTML files. Neither of these browsers support arbitrary code execution, and Gopher is fine with that. Everything works the way it was supposed to. 

See, Gopher can work just like the web, minus all the parts of the web that are bad (tracking, unwanted downloads, arbitrary code execution.) and minus a few parts that aren't bad (most gopher sites do not support links in any place other than in menus, although this is more of a limitation of the browsers than the servers. Also, all gophersites look the same, which is to say, ugly.) 

It is Ugly. Ugly isn't bad. It is utilitarian. It's more useful. It's less harmful. It's even more accessible to screen-readers, and entirely keyboard navigable, if you're in an actual gopher client. That's GREAT for people with motor control problems, or people with vision impairment. 

Now, hearing this, you might be asking yourself: How can I expereince Gopher? The short answer is to install a Gopher browser. The long answer is less thrilling. 

See, modern Gopher clients exist, but not many of them, and they are all incomplete or works in progress. The best one I've found so far, if you don't need it to support images and you're on a Unix-like system, is Lynx. If you're on Windows try [GopherBrowser](http://www.jaruzel.com/apps/gopher-browser-for-windows/), and on [Android there's Overbite](http://gopher.floodgap.com/overbite/d?android). Everywhere else, use the [floodgap proxy](http://gopher.floodgap.com/gopher/), and expect it to be slow. 

The good gopher clients are... well, they are relics mostly. Like, written almost 30 years ago and barely changed since then. It'd be like if web browsers had never gotten any better than IE 5. Actually, no, it's worse than that. IE 5 wasn't released until 1999. The state of gopher clients is that they essentially haven't changed since Windows 3.1. No progress since ~1994. 

I've been talking to some folks on the internet (mostly, via [mastodon](http://retro.social)) about the problems with the web, and the potential of Gopher as an antidote. Specifically, if we redesigned the Gopher client, and fast-forwarded it through ~30 years of technological progress. 

We're gaining some traction! There's rumblings of writing a new, better, modern Gopher browser that has all the trappings of a modern web browser, but doesn't do arbitrary code execution, and only downloads what you tell it to, and exactly what you tell it to, no more. 

So you'd have menus that open up Markdown or HTML pages, and those pages could link to other menus, or to files directly. You'd have optional image support. The pages themselves could even have some basic styling! But HTML and Markdown aren't actually programming languages, they can't do dynamic stuff, so it's safe(er) to do! 

And, if we do it well, and we foster the right kind of community of publsihers, there's no reason why the modern gopherspace can't be shared and enjoyed on everything from the latest and greatest smartphones to the 8-bit computers hanging out in your grandparent's attic. The protocol is dead simple, and as long as we make sure to offer Plaintext (or markdown) alongside the fancy files, it'll still work for everyone. 

If somebody actually pulls it off, then there's still the problem of convincing the world to start publishing on Gopher again (but [SDF does](http://sdf.org/?tutorials/gopher), and [Tilde.Town](http://tilde.town/) does, and Wikipedia does, and Metafilter does, and any website with an RSS feed (read: most of them) can be converted in to a gopersite pretty simply, with or without the support of the original owner of the content.) It'll likely never be more than a niche thing, but being around for (and involved in) the genesis of this resurgence, if it ever amounts to anything, is kind of neat. 

So, what do you think? Is Gopher the answer to the problems of the modern web? Do you have a better idea? 

I'm on Mastodon [@ajroach42@retro.social](https://retro.social/@ajroach42), and I'd love to hear your thoughts. 
