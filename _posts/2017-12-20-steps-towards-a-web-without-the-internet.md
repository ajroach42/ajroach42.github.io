---
layout: post
category: post
published: true
title: Steps Towards a Web without The Internet
---
[The web is broken.](https://www.neustadt.fr/essays/against-a-user-hostile-web/) We've talked about this before ([net noot](http://ajroach42.com/net-neutrality-the-consolidation-of-american-media-and-you/), [gopher](http://ajroach42.com/gopher-remembering-the-web-that-wasn-t/)). Today, I am here to talk about some potential solutions. Specifically I want to talk about how we can leverage some brand new technologies to build a network that operates independently from the Internet and supplements it, mitigating the ways the web is bad for users.  

A little over three years ago, I wrote an article for the [Analog Revolution Magazine](http://analogrevolution.com) abouty the Alternet, a wacky project we were running up at the record store. 

We didn't have an internet connection at the store, so we set up a little box that wasn't connected to the internet, and we served some web pages, some public domain movies, a message board, and a chatroom, all over local wifi. 

If you were in the store or at the attached venue you could connect and share files, watch movies, and elave messges on the server. 

Basically, it was a BBS. 

In February of 2016, I gathered some thoughts on that project into [an article about building a Modern BBS](http://ajroach42.com/a-modern-bbs/). It is consistently my most popular article, and honestly one of my favorite topics. I talk about ways to fix and expand on the mBBS concept pretty much every day. 

There were some problems with the project. First, it was *very* local. I mean, it only really worked if the users were in the same building as one of the nodes. Syncing between the nodes was supposed to be handeled via sFTP and rsync, but in practice it was an ugly mess that didn't work and would have been easy to abuse. 

But this isn't about the past. 

This is about taking those ideas, and expanding on them, turning them in to a new, modern, encrypted, internet adjacent networking platform. 

Exciting, right? 

## Alll about dat DAT 

The biggest news on this project is probably [Beaker Browser and DAT](https://beakerbrowser.com/). There's a lot to unpack here, but I'll try to hit the highlights. 

### DAT 

- Technically, DAT is a protocol for distributed, peer-to-peer file sharing with version history. 
- Basically, DAT is a new kind of torrent, but with some secret sauce.
- They merged the idea of a torrent with ideas from [Secure Scuttlebutt](http://scuttlebot.io/), and the end result is a torrent that can be modified by it's creator. 
- Importantly, they do all of this without requiring "proof-of-work" 

### Beaker 

- Beaker is a web browser that lets you interact with DATs like they are webpages. 
- Beaker also lets as a way to create/host DATs. 
- Once you have created a DAT, anyone who visits it can re-host it. 
- If you make changes, and they are online, their version will update automatically. 
- This does not require an internet connection, and can be done entirely peer-to-peer over an intranet. 

I want to take advantage of that. The principal problem that prevented our servers from becoming a network was syncing between nodes. Content published on one node did not easilly sync to other nodes, and bi-directional sync was almost impossible. 

DAT can solve some of these problems. 

## Proof of Concept 

I did some really basic testing with DAT/Beaker last night and this morning to see if it could work as a sync method for our mBBS. 

For my test: 

- I set up a local intranet (using the old mBBS box from Analog Revolution) 
- I connected three computers to it. 
- Using one of the computers I published a DAT, and put a link to that DAT on the intranet homepage. 
- Using another one of those computers I opened the DAT and added it to my library. 
- I shut down the first computer. 
- I opened the DAT using the third computer, via the second computer. 
- I then connected computers 1 and 2 to the internet. 
- From Computer 1, I made changes to the DAT. 
- They were automatically updated on computer 2! 
- I disconnected computer 2 from the internet, and reconnected it to my intranet. 
- Computer 3 updated automatically!

So, I called that a successful test. 

## Putting it all Together  

If I understand everything correctly, this can work. If it does, it will work like this: 

- Users connect to the alternet over wifi from the computers or phones or tablet. It is an open wifi network. 
- This will open up to a homepage that serves as a directory of all the services and pages available from this node. 
- All users can interact with all the pages available from the BBS through their regular web browser, etc, all http traffic is public and unencrypted.
- Included in these pages are applications for chat and video sharing and all kinda stuff. 
- If those users have Beaker or another DAT browser installed they can interact via DAT instead. 
- When they interact via DAT, they can choose to sync pages from this BBS to their computer. 
- They can publish files
- Published files can be available over DAT only while they are connected to the network, **or** they can submit the DAT address to the BBS so that the BBS will peer that content and continue to make it available once they have disconnected.
- Then, if they connect to another BBS, it will bidirectionally update any pages that are available in both places. 

It looks like there will be a way to upload content over HTTP, too. That'll be less needed as more DAT browsers are released, but it serves as a nice stop gap for now.

Based on all of that, this means that the nodes don't have to be connected to one another directly, mesh or otherwise. The users can sneakernet the data back and forth simply by accessing it. 

However! If the nodes can be connected (over the internet, over a temporary long range connection, over a phone line, over RF, via flash drives, whatever) the DAT protocol will also handle those syncs, thus preserving data integrity and reducing the potential for man-in-the-middle attacks.

Further, while http traffic will be unencrypted as a result of there not being a certificate authority available, DAT traffic is encrypted by default. DAT can even be used to serve updates for the server software, and to verify their authenticity. This simplifies the update proccess, and helps ensure servers are not compromised. 

It's not a perfect solution, especially because there are no good DAT clients for android and ios, but that situation is temporary, and allowing for HTTP fallback is not particularly problematic as a short term solution, IMO. 


## Next steps 

The next step is to get DAT, which is based on node.js, installed on a clean Raspberry Pi. From there, I just need to build a simple web-app thing that will run on the BBS box, serving as it's homepage. That app should:

- accept DAT URLs + metadata via a form
- Publish links to those DAT URLs (and meta) to the BBS homepage 
- Peer each of those DATs from the BBS box (provided it has enough room) 

That page will be served over HTTP and DAT and all the pages the BBS peers would also be made available over HTTP and DAT, at least until mobile devices have good DAT browsers. 

## Further Reading 

- [Dat Documentation](https://docs.datproject.org/) 
- [Using Beaker](https://beakerbrowser.com/docs/using-beaker/)
- [Against an increasingly user hostile web](https://www.neustadt.fr/essays/against-a-user-hostile-web/)
- [Rescuing the Web from the Internet](https://staltz.com/a-plan-to-rescue-the-web-from-the-internet.html): A more ambitious plan to leverage some of the same technologies to build a more long-term network.
