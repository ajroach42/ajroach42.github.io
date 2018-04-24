---
layout: post
category: post
published: false
title: 'Observations on Modern Computing (The Last 10 Years Were a Misstep) '
---
I make no secret of the fact that I love [old computers](http://ajroach42.com/a-modern-office-with-vintage-hardware/), and that I think modern computers have lost their way in terms of providing utility to users. To that end, I write about, and think about, computers and the way to move computers forward, without losing site of the fact that computers should serve their users. I grew up with hand-me-down computers, from Atari to Apple (II GS!) to Dell, and in the process I got to experience a sizable portion of computer history very quickly, in my teen years. 

This left me with Opinions. 

I write about things that are informed by these opinions often. When I talk about building a [World Wide Web analog without the internet](http://ajroach42.com/steps-towards-a-web-without-the-internet/), about [reviving the BBS](http://ajroach42.com/a-modern-bbs/) or when [I lament the fact that Gopher was doomed to obscurity by the modern web](http://ajroach42.com/gopher-remembering-the-web-that-wasn-t/), it is in response to my experiences with an array of computers from the dawn of the home computer revolution up through to the modern age. There was a time when computers were magical. 

I had come, in recent months, to suspect that I might just be an old fuddy-duddy. I'm approaching 30 years old, and I was beggining to feel like I was looking at modern computers and modern software through the lens of someone who was being left behind, shouting at the sky, shaking my fists at the kids on my lawn. I was coming to the conclusion that my love of these computers of my childhood, and of ones that I had never had the chance to interact with, was some kind of rose tinted nostalgia. I had not fully subscribed to this theory, but it seemed more likely that I was romanticizing something that was actually Not Great that it was that nearly every modern software and hardware platform had inexplicably gotten shittier. 

I am now prepaired to say, with conviction, that every modern hardware and software platform has gotten shittier, and that it's not inexplicable. I'm going to try to explain how I came to this conclusion, and give some potential explainations. 

## About Me 

First, let me lay out a little bit about my technical literacy and my profession, this might help explain some of the assertions that I'm going to make. I started using computers, and the internet, in 1995. Our family computer, my first computer, ran Windows 3.11 (for workgroups). Later, in the late 90s, I was given an Atari 400 and reams of books and magazines on basic, followed shortly by an Apple II GS and dozens of disks of software. Later still, I started collecting computer detritus, and assembling frankenstiend linux boxes, and emulating some of the the machines I read about in the magazines I had as a kid. 

I loved computers. I loved making weird little programs, and silly applications and games. I'd build things in GW Basic or Freebasic, and distribute it to my friends on floppy disks. Even in the latter half of the 00s, I was passing half broken games around on floppy disks (or collections on CD-Rs, when I could talk someone in to buying some for me.) Computers were, by and large, ubiquitous in my life. Nearly everyone had an old one they didn't want, and a new one they didn't understand. For a teenager and an aspiring computer programmer, it was a great time to learn. 

I collected cast offs from neighbors, from thrift stores, from office upgrades. I rebuilt them, installed useful or fun software on them, and sold them or gave them away. All of my friends had computers of their own, because I had access to these machines, and I cared enough to outfit them with the appropriate software. (It must be said, at this point, that 'useful' and 'appropriate' are relative terms. In 2009 I gave a good friend a computer that had been built for Windows 98. It was running Puppy Linux from a CD, and saving data to a USB flash drive over USB 1.1. It did word processing, email, and basic web browsing. It had a whopping 64MB of RAM, and was covered in glitter, googley eyes, and carpet samples. But it was free, and it wasn't useless, and that was important.)

I went to school to become a programmer, and discovered that I don't enjoy programming as it exits today. I understand it well enough, and I *can* do it, but I don't *want* to. I make websites, and I build tools to help other people use computers. I make my living as a systems adminstrator and support engineer. (and I'm looking for a new gig, if you're hiring.) That's a fancy way of saying that I solve people's computer problems. Professionally, I'm responsible for identifiying and mitigating the shortcomings of various computer systems. 

Guess what? 

There are a lot of these short comings. Like, a lot. More than I ever expected. 

Some of these shortcomings are legitimate bugs. Some of them are bafflingly shortsited or poorly considered architectural decisions. Just as many are cases of a divergence between the needs of the user and the abilities of a program. Modern programs are often feature incomplete, poorly supported, and difficult or impossible to customize. Modern computers are often slow, and cranky. I'm responsible for handling the fallout of this unfortunate situation. 

I've seen how revolutionary a computer can be, if it is designed with the needs of the user in mind, and how disasterous the same can be when it is not. I've seen computers used to empower people, and used to opress. I've seen computers be Good, and the consequences of when they are not. 


So that's who I am, and my experience with computers so far. Those are my credentials, and my qualifications. 

## Computer Chronicles 

Before we go any further, let's talk about The Computer Chronicles. This was a TV show that ran from the early 80s through the early 00s. Over it's nearly 20 year run, The Computer Chronicles covered nearly every fascet of the newly developing Computer industry. It was hosted by people with Opinions. The guests were, frequently, people who were proud of the things they made, or the software they represented. Watching the developer of CP/M and DR DOS talk to a mainframe engineer who worked at IBM in the 50s about the future of computers as seen from the 1980s was eye openning. 

<iframe src="https://archive.org/embed/MainFram1984" width="640" height="480" frameborder="0" webkitallowfullscreen="true" mozallowfullscreen="true" allowfullscreen></iframe>

On the one hand, this show serves as an excellent introduction to, or reminder of, the capabilities of computers 35 years ago. It helps us see how far we've come in terms of miniturization, while also demonstrating again that, in many ways, there is nothing new under the sun. Before the advent of the internet, reporters were writing their stories on laptops and sending them in over phone lines, 25 years before the release of the iphone HP released a computer with a touchscreen, three years before microsoft released he first version of windows Apple and Visicorp demontrated GUIs wih features that Windows wouldn't be able to approach for another 9+ years. 

And, of course, I'm reminded again of Douglas Engelbart's 1968 "Mother of all Demos", in which he demonstrated the mouse, the GUI, instant messaging, networked gaming, and basically every other important development of the following 50 years. 

<iframe src="https://archive.org/embed/XD300-23_68HighlightsAResearchCntAugHumanIntellect" width="640" height="480" frameborder="0" webkitallowfullscreen="true" mozallowfullscreen="true" allowfullscreen></iframe>

It took 5 years for Xerox to refine and miniturize Engelbart's ideas to the point that they thought they could market them, and another 10 years before Apple refined and further miniturizaed the same ideas, and brought us the Mac. 

Nothing new under the sun. 

The whole video of Engelbart's Online System (NLS) is available on archive.org, along with a ton of other [video content from Engelbart](https://archive.org/details/dougengelbartarchives). Some of it is *really* interesting. Most of it is unfortunately dry. It's easy to forget that this was 50 years ago, and also mindblowing that it was only 50 years ago. 

Anyway, back to Computer Chronicles. In an episode about Word Proccessors, the man they were interviewing said "There's a lot of talk about making people more computer literate. I'd rather make computers more people literate." There's a phrase that resonated with me in a big way. 

It sounds like the kind of symantic buzzword shuffling so common in standard corporate speak, but I got the impression that the guy that said it, believed it. He believed that computers had gotten powerful enough that they no longer had to be inscruitable. 

## The Scruitable Computer 

There were others working around the same time on similar ideas, or at least from a similar philosophy. Working to make computers, if not intuitive, at least comprehensible. I think this is a noble goal. 

The computer is often thought of as a tool, but it is more like a tool shed, in which we store a collection of tools, a source of power, and a workspace. The tools of the 60s and 70s were primative, partially because of the limited space and limited power our toolbox could provide for them, but also because our ideas and understanding of how these tools should work were limited by the audience who was using the tools. 

That is to say, in the 60s and 70s, computers were weak and slow and computer users were also computer programmers. A small, tight knit circle of developers and computer scientists were responsible for the bulk of the progress made in that time, and the idea of designing tools for non-technical users was never considered. 

Computer culture had, by and large, a kind of ellitism about it as a result of the expense and education required to really spend much time with a computer. This changed, slowly, starting in the mid 70s with the development of the Microcomputer Market and CP/M. 

Computers became more affordable, slowly. Affordable computers became more powerful, quickly. Within 10 years, non-technical users were interacting with computers on a daily basis. It was against the beginnings of this backdrop that the phrase I mentioned earlier was coined. "Human Literate Computers" or "Human Centered Computing."

Ease of Use was the holy grail for a lot of computer companies. A computer that was so easy to use that they could sell it to grandma. But, to me at least, Human Literate and Easy to Use are distinct ideas. Many modern applications are Easy to Use. Netflix is Easy to Use. Facebook is, for all it's faults, pretty easy to use. The iPhone, the iPad, and ChromeOS are super easy to use. 

Well, they are easy to use as long as you use them in the prescribed way. As long as you let them tell you what you want to do, instead of the other way around. 

That, in my opinion, is the distinction.

## Why didn't it work? 

I think that many of the steps towards demistifying the computer of the 80s and 90s did good work, but ultimately, the computer industry left the whole idea behind, in favor of making some tasks Very Easy while making other tasks Practically Impossible, and turning everything in to a survielance device. It seems like every major advancement over the last 10 years has been, at best, a step in the wrong direction. 

But this isn't about Programming Tools or about Ease of Use. It's about the idea of User Friendliness, and the competing idea of User Hostility. Modern computers are Intentionally user hostile, in that the modern internet is a survielance machine, but modern computer are also user hostile in that we don't provide documentation on our software, and we no longer make our software end-user modifiable. 

So let's define "User Friendly". A User Friendly computer: 
- Respects user's privacy, only collecting data that is required, and only storing it for as long as it's needed 
- Does what it says that it's doing
- Is designed using consistent design language and operating paradigms 
- Doesn't waste time, power, bandwidth, or battery life needlesly 
- Is well documented 
- Is end user modifiable (this includes hardware, such as increasing RAM or storage, and software. I should be able to run my own software at a minimum, but further than that, I should be able to modify all the software I run to meet my needs.)
- Does not make simple tasks needlessly complicated
- Does not prescribe to the user how it should be used, instead letting the user make substantative descisions about how the machine will work
- If it must fail, it gives the user as much information as possible about the failure 
- If it must fail, it is obvious that it has failed 

Modern computers, and modern software, fail on nearly every one of the above counts, almost all the time. In many small ways, computers and software have improved so far beyond what we would have imagine that they were capable of 20 years ago, but the gains are unevenly distributed and hidden behind layers of user hostile behavior. 

I've read lots of arguments that what I'm calling user hostile behavior is actually just the economics of the modern computer industry and... yeah! The economics of the modern computer industry are user hostile. Users are rarely customers, and are instead products. Even in the FOSS world (and, let's be clear, I have a lot of love for the FOSS world but it is not without flaw) the dominant business model is "the software is free, pay for the support", we can call this the Red Hat model. 

The Red Hat model produces a perverse incentive to keep the software complicated, and the documentation inadequate. This is not a universal rule, and I'm certain that Red Hat has contributed more to User Friendly computing than they have taken away, but not every company engaged in this model is equally altrusitic. 

## What can we do?

We, as users, as creators, and as people, have an obligation to help fight back against this. We can: 
- Make user friendly (not user hostile) devices and software 
- Write documentation 
- Refuse to buy tech that *we* can render safe to use, but that the average user can't
- Support finanically the people and organizations taht produce user friendly hardware and software whenever possible.
- Write to our congresscritters about the DMCA (a law that is wielded by the likes of Lexmark and John Deere and Microsoft to keep their devices user hostile by rendering it illegal to install your own software.) 
- Normalize the idea that reading documentation is sometimes required, and in the process, help folks bridge the gap in computer literacy.
- Encourage tinkering and customization by documenting all the ways that it is possible. 

Part of this is very difficult, because documentation requires a separate skillset than development. If you are good at writing engaging and understandable documentation, consider finding a project to which you can donate or sell your services. If you run a software project (FOSS or otherwise) consider finding a technical writer, and value their opinions and input (and, while you're at it, hire a designer. Their contributions will be invaluable.)

And, of course, keep talking about, thinking about, and building user centric systems.
