---
layout: post
category: post
published: false
title: Jupiter's Ghost - Cartoon PILOT
---
<iframe title="Jupiter's Ghost [PILOT] - Generational Mice" src="https://vod.newellijay.tv/videos/embed/85ea7ad6-e603-490f-aba9-20debfc06c59" allowfullscreen="" sandbox="allow-same-origin allow-scripts allow-popups" width="560" height="315" frameborder="0"></iframe>

As I mentioned in an [Earlier Post](https://ajroach42.com/announcing-jupiter-s-ghost/), in fits and spurts over the last decade, and with some dedication over the last several months, we've been working on a colaboartive, crowd sourced, creative commons licensed [podcast](https://intergalactic.computer/social/podcasts/) set in the shared Solar Federation universe called [Jupiter's Ghost](https://intergalactic.computer). Today, here's a sneak peak at what this podcast might look like as a [Cartoon](https://vod.newellijay.tv/w/hx7PGjW5YqTG8c6q4nrD7R). It's a little rough around the edges, but I think it's a great pilot. 

I put this episode out, warts and all, because I think it's pretty good, and I think it gives the impression of what could be in a meaningful way. I could have put another 10 hours in to it, but I don't have another 10 hours to spare in the next three weeks. It was now or three months from now, and I chose now. 

Having seen the finished result, I'm almost sold on the idea of doing a regular cartoon from this podcast, but I want to see how it goes over with the rest of our community first. I'm going to wait and see what the rest of the Jupiter's Ghost crew and the rest of the New Ellijay Television crew have to say about it, but I think we've come pretty close to cracking the minimum viable TV show.

# What? 

[Juptier's Ghost is a podcast](https://intergalactic.computer)! This is a kind of companion to the podcast for folks who prefer to see things on screen. And, to be clear, it's rough. If we graduate this show from a pilot through to an ongoing series, it'll look a little different, and it will be a little more dynamic. IF you like it as is, or you think you might like it with 30% more polish, please do let us know. 

# How? 

The character animations, such as they are, were done in Adobe Character animator. I hate using Adobe products, and I'm exploring some other propritary animation software to see if it will meet our needs. I was disappointed to discover that Adobe really seems to have a lock on the idea of modern/digital limited animation. There is no libre option that I could find with automatic mouth and head movements, or simple puppet/rigging based 2D animation, and I don't have the time and energy to become a full time animator. 

Aside from drawing and rigging the puppets (or, in a few cases, using Adobe's Puppet Builder), the actual process of building these animations just took a few minutes. You feed the software an audio file, click two buttons, and wait a minute or two. In an ideal world, you then watch back through the rendered animation and do some cleanup + add some more dynamic motion (you can see an example of that in the last log from James Andrews, which was our first attempt, and got an extra 20 minutes or so of work.) If we continue to do episodes like this in the future, we'll do all new original puppets, and we'll rig them to be a little more advanced (that is to say, walking, head turning, multiple static poses, etc.) and we'll take the time to more fully animate each character per scene. 

The show will still be fairly static, as it will still be built from the podcast and that means mostly characters talking to camera, delivering reports. There's not much to do with the camera, and not very many interesting ways I could frame the monologues to make them more visually dynamic. We could do more background animation, make the ship feel a little more lively, but it's still going to be long shots to camera. 

Outside of Character Animator, the vast majority of the work was done in [Kdenlive](https://kdenlive.org/en/). I like Kdenlive a lot, it's a robust video editor with some powerful features, it's free, it's fast, it's reasonably stable, it's cross platform, and it doesn't spy on me or send my work to some remote server for [Content Analysis](https://www.dpreview.com/news/6341509927/adobes-content-analysis-program-raises-privacy-concern). All the background and foreground images, intro titles, and effects were composited in kdenlive. Most of the static images came from [ansimuz](https://ansimuz.itch.io/) on itch.io, and any required modifcations were done in Krita. 

We'll post more about KDEnlive in the future, because we really put it through it's paces on the upcoming episodes of Shouting into the Void, and I'm pleased to share what it's capable of. 

Once I had the background and foreground images, episode content, and basic puppets, going from assets to epiosde took somewhere in the ballpark of an hour. That includes color grading, animating, building titles and effects. 

Rendering the thing took ... Longer than I expected, considering the hardware it was rendering on, but we did really layer on some effects and KDEnlive isn't *really* designed for this kind of manipulation of static images. I think the rendering procces was averaging 28 minutes for this episode using VAAPI acceleration on a 3080 TI, and about 30 minutes on a Ryzen 9 CPU. I could likely speed that up by moving our assets to the SSD, and/or precompositing some of the more complicated effects (that is to say, editing the backgrounds and rendering them out to a high quality file, then inserting that composited video under the foreground animation.) 

Regardless, it worked. It looks okay, and it didn't take a huge amount of time. 

## Next steps 

As I said above, this is not a finished, polished thing. If the reception is good, we'll get new original puppets for every character, design some original backgrounds for a few Key locations on the ship + generic hallways and crew quarters that we can decorate for individual characters to give the ship a more coherent style and feel. We'll also spend more time on the actual animation, to ensure that it's smoother and a little more dynamic. 

We'll accomplish those things by having *someone else* do them. The biggest thing I learned from working on this project is that I rarely have 5 hours of uninterrupted time, and that I would be better served using my time elsewhere. There are a lot of people working on Jupiter's Ghost and New Ellijay Television and this project would be better served in the hands of some of them. 

So what do you think? Is it worth going down this road? What would you do differently? 