---
layout: post
category: post
title: 'Be Your Own Netflix: a "Why To" on running a personal streaming server'
published: true
---
This is a post about running your own streaming media server, and why you might want to do that. I will discuss some surface-level strategies for how you might go about it, and how you might source media to fill it with, but this is not a step-by-step guide. It's a "why to", rather than a "how to" So hop in, and let's talk about streaming media in 2025, and what you can do to take back control.

In [the last post in this series](https://ajroach42.com/unplugging-the-beast-leaving-disney-hulu-and-the-rest-of-the-streaming-oligarchy/) I talked at length about why you might want to leave existing corporate media platforms. I won't re-hash all of those arguments here, but I'm going to assume if you're reading this that you already have your reasons. Maybe you're tired of the censorship, the price hikes, or the feeling that your favorite show might vanish into a licensing black hole. Instead, in this post, I'm going to talk about why you might want to self-host a media server instead of simply availing yourself of other available alternatives.

### Why Self Host? 

In this era of streaming, we've grown accustomed to certain modes of interaction. Even if you have a big physical media library, you may want to be able to access it on the road, or from your smart TV, or maybe you just don't want to have to get up and insert a blu-ray or a DVD. A media server brings that convenience home, literally.

But it's more than that. Self-hosting is an act of declaration. It's saying, "This is my space. These are my stories." Here’s why that matters:

*  **It's Yours, Forever:** When you buy a DVD or a DRM-free file, you've purchased a license to that media. A server is how you exercise that license on your own terms. No corporation can take it away, edit it, or bury it in an algorithm. Your library is permanent.
*  **The Great Unifier:** If you support independent cinema you might also find yourself, like me, in the position of having a large number of legitimately acquired DRM-free digital downloads from various Kickstarters, Indiegogo campaigns, and other crowdfunding efforts. Keeping track of and consuming bare digital files is, frankly, a pain in the butt. A good, self-hosted media server can make that more pleasant. It also seamlessly integrates your physical media rips, home movies, and any other digital files into one beautiful, browsable interface.
*  **A Sanctuary from the Noise:** Your server has no ads. No "trending now" algorithms vying for your attention. No data being mined about whether you binge cartoons on Tuesday nights. It's a quiet, intentional space for the content you have consciously chosen to bring into your life.
*  **Digital Stewardship:** You become an archivist. By ripping your discs and saving digital files, you're taking some steps towards ensuring the art you love survives platform decay and corporate whims. You're preserving a piece of culture in a small, personal, but very real way.
*  **It Just Works Better (For You):** The user experience, when tailored to your own collection, is simply superior. No more jumping between six different apps with six different interfaces. Everything you care about is in one place, organized exactly how you want it, ready to play the second you hit the button.

### Jellyfin, Kodi, or Something Else? Picking Your Poison

For me, there are two good options for server software, one okay option, and one I'd avoid.

**[Jellyfin](https://jellyfin.org/): The New Standard**
Jellyfin is the new kid on the block, and it's excellent. It's completely free and open-source, with no "premium" features held back. It's incredibly powerful, with apps for virtually every platform (Roku, Fire TV, Android, iOS, etc.). It automatically fetches beautiful metadata, art, and subtitles. If you're starting today, **Jellyfin is probably your best bet.**

**[Kodi](https://kodi.tv/): The Grizzled Veteran**
Kodi has a long and storied history, evolving from the legendary XBMC. It's more than just a server; it's a full-blown, highly customizable media center interface. Its strength lies in its immense ecosystem of add-ons and skins. It can feel a bit more complex to set up for whole-home streaming, but it's a powerhouse for the dedicated tinkerer.

**What about Emby?**
In my last post I mentioned Emby briefly. It's the open-source project Jellyfin was forked from. It's slick and has a good reputation. However, it operates under a freemium model, with some fairly significant features like hardware transcoding locked behind a paywall. I don't love this kind of artificial limitation on technologies I'm hosting myself. It's a valid option, but I have reservations.

**And Plex? A Caution.**
I expect Plex to fully [enshitify](https://doctorow.medium.com/social-quitting-1ce85b67b456) itself at any moment. It has a broad feature set, it works well, and it's (sort of) self-hostable. But nearly everything you do is tied to Plex's servers, and I am very suspicious of their motives and the amount of data collection they do. I used Plex years ago but have since migrated away and encourage you to do the same.

### Hardware: Keep It Simple

Lots of these tutorials say something like "run it on a raspberry pi" and ... I mean you can, if you know what you're doing and you want to use underpowered hardware for this purpose, but I wouldn't.

My strong recommendation? **Run it on an old laptop.** It's the perfect home server: it has a built-in battery backup (a huge plus), a screen for setup, and is designed for low power consumption. Hook it up to a large external hard drive—something like a Seagate Expansion drive which holds 18TB of media and represents a great dollar-to-byte ratio. You could probably get away with something much smaller, but the principle stands.

Pick whatever software you want. Run it on whatever hardware you have. Don't think about it too much, unless you really want to, in which case you should probably be reading a different, much longer post.

### Fancy Networking: Reaching Home From Everywhere Else 

The following section touches on some technical topics, but doesn't get very deep into them. If you want to access your media server from outside your home, you might need to look at one of the techniques discussed here. You may need to research one of these topics in more detail, even. 

If you don't need to access your server from outside your home, skip it. No hard feelings.

My goal is to introduce complex topics and keywords, giving you enough of a foundation to adapt this for your own situation or use it as a springboard for further research.

The biggest benefit to something like Plex or Emby over Jellyfin is the perceived ease of remote access. This is true, but it's also non-essential once you know the alternatives.

*   **The Simple, Magical Way: ZeroTier.** Think of ZeroTier as a "magic tunnel" that creates a secure, private network between all your devices, no matter where they are. Install ZeroTier on your server and your phone/laptop, have them all join the same network. [The whole process is documented on their site, and takes about 2 minutes](https://docs.zerotier.com/quickstart/). Now, you can access your Jellyfin server from a coffee shop as if you were on your own couch. It's dead simple to set up and free for personal use. This is my go-to recommendation.
*   **The Advanced, "Full Internet Citizen" Way: A Reverse Proxy.** This is what you'd need if you want to let your friends access your server from their homes without installing any special software. It's a way to securely open a single, specific door from the public internet into your server. The steps for doing this, and the security considerations, are beyond the scope of this article. The simple version is: 1) have a server with a static IP address join your Zerotier network 2) [configure your server software to proxy connections back to your home network](https://jellyfin.org/docs/general/post-install/networking/reverse-proxy/nginx/).

There are services, both free and paid, that exist to provide a quick and dirty dynamic subdomain and reverse proxy for your home network. I've used several over the years, but these days I just have a $2.50/month server from Vultr that does the work for me.

**Important note:** if all the networking stuff made your eyes gloss over, that's fine. Not everyone needs to understand home networking. If you don't need to access your media server when you're away from home, skip it. If you do, but you didn't understand the networking, I can point you towards some good tutorials, or help you when you get stuck. This kind of thing isn't *easy*, but it is achievable, even without a technical background.

### The Media Itself: The Treasure Hunt

Alright, that's most of the boring technical stuff out of the way! Now let's talk about the fun part: a few strategies you can use to load up your server with media.

**1) Physical Media**
I love physical media, but the first thing I do when I get a new DVD or Blueray is rip it. I personally use [MakeMKV](https://www.makemkv.com/) for this task, which does the job admirably, and is currently free to use. MakeMKV will also work with 4K/UHD discs, but you'll need a [drive with the appropriate firmware](https://forum.makemkv.com/forum/viewtopic.php?t=19634).

[Handbrake](https://handbrake.fr/) can also do DVDs, although it might run into trouble with encrypted DVDs. If you do, you're probably on Windows and you'll [probably need a copy of libdvdcss.dll](https://github.com/allienx/libdvdcss-dll/releases).

Depending on where you live, it may or may not be legal for you to break the encryption on your DVDs or blurays, but it *is* legal to back up those discs in most jurisdictions. It's a practice known as format shifting, and it has been routinely supported in both written and case law. This mess is, in the US at least, because of the DMCA. The DMCA was a bad law that should not have been passed. 

Of course, your mileage may vary, I am not a lawyer, etc. etc. etc.

**2) Kickstarter and Indie Downloads**
A lot of kickstarters for new films and TV shows and for silent film restoration and other public domain archival come with a DRM free download.

Often times these will be delivered via Vimeo. If it looks like it doesn't have a download and is just streaming on vimeo, double check. Often there is a "download" button hiding on the page somewhere.

**3) The Internet Archive and Wikimedia Commons**
Speaking of the public domain, the [Internet Archive](https://archive.org/) has a large repository of public domain material. Now, a critical note: **just because it's on the Internet Archive does not mean it's in the public domain.** There's a [huge amount](https://archive.org/details/space-patrol) of [legally available](https://archive.org/details/bugs-bunny-pd-cartoon-collection) [public domain material](https://archive.org/details/his-girl-friday-1940) on the archive, but there are also [ a fair number of things that probably shouldn't be there.](https://archive.org/details/ikaos-som-dragon-ball-complete-001-153-r2j-dragon-box-multi-audio-v4_202301/Dragon+Ball.001.DBOX.480p.x264-iKaos+%5Bv4%5D+%5BCED9F4DB%5D.mkv)

The Archive is a particularly good resource for early public domain television episodes, classic films, and obscure newsreels. **All of these items are available via BitTorrent.** You can find a "Torrent" download link on the item's page, which you can feed to your torrent client. Downloading public domain content via torrent from the Internet Archive is a perfectly legal and efficient way to acquire these files, unlike getting your torrents from a site like [1337x.to](https://1337x.to), which hosts primarily infringing content.

Wikimedia Commons also has a huge number of public domain films, such as *[Filibus](https://commons.wikimedia.org/wiki/File:Filibus_1915.webm)* and *[Charade](https://upload.wikimedia.org/wikipedia/commons/e/ef/Charade_%28Stanley_Donen%2C_1963%29.webm)*, ready to download directly.

Both services are also home to lots of music, including Public Domain recordings, and CC licensed material from various netlables. I'll talk more about music in a future post. 

**4) PeerTube**
Most videos hosted on PeerTube have downloads enabled. I have a huge library of public domain and creative commons licensed material on my own instance. You can visit [New Ellijay Television](https://vod.newellijay.tv) and press the download button on any of our videos. (Here's one to get you started: [The First Spaceship on Venus](https://vod.newellijay.tv/w/wK4UoQwukx5gf6mTgh6Ak8).) 

If that gets tedious, you can also use [yt-dlp](https://github.com/yt-dlp/yt-dlp) on PeerTube (along with [lots of other services](https://github.com/yt-dlp/yt-dlp/blob/master/supportedsites.md)) to download materials that are legal to download. It works well and will download a whole playlist or channel if that's what you ask it to do. If you're going to use yt-dlp, wrap the url in quotes. So the command to download every video from our music channel would be: 

`yt-dlp "https://vod.newellijay.tv/c/music/videos"`

It can be intimidating to use at first, but once you get used to it it is very simple.

**5) Other sources**
In the near future, I'll be writing up a more comprehensive guide to building a digital media library from legal sources. But nothing will ever be truly comprehensive, so I encourage you to seek out other sources.

> **An Important Distinction:** I have not mentioned copyright piracy here, because it is illegal in most jurisdictions. It is, however, worth noting that some of the tools I mention, like yt-dlp or torrenting, can be used for both legal preservation and illegal downloading. Pay attention to what you're doing, and make sure you are legally covered.

### Cleaning It Up: The Final Polish

Once you've got your media on your server, you're going to want to make sure it matches the naming conventions your software expects. If your TV shows aren't in folders like this: SHOW NAME > SEASON 01 > FILE they probably won't show up in Jellyfin. There are tools that'll help organize things if you're having a hard time. I like [Mediaelch](https://www.mediaelch.de/mediaelch/). It's a free tool that you can use to sort and rename your poorly named media. It's not as fast as some of the paid options (like Filebot), but it works well enough for most people in most cases. 

Your server software will usually automatically fetch poster art, descriptions, and other metadata. If it doesn't, it might not be able to identify what a piece of media is. That's fine, you can either fix it by helping the server identify the media, or by manually adding images, descriptions etc.

### And Then What?

Well, if you've made it this far, you'll have a home media server with a growing library of content that you can watch or listen to when you're at home. If you set up zerotier (and I think you should!) then you can also access it from your phone or laptop when you're on the road. And if you got real deep in the weeds with a reverse proxy, you can even let your friends access your server from their homes.

In future posts, I'll discuss other places from which you can find media, turning this library into a live streaming television network (complete with commercials, if you want them), and how to make it easier for your friends to add videos to your library.

Until then, have fun and happy watching. You've just built something that can't be taken away from you.
