---
layout: post
category: post
published: true
title: DeOldify - Automatically colorizing videos
---
Whew, what a year! I bought a computer in March with the intent of using it to do some video processing and film preservation work. Then ... well, this year happened. Last night, I finally finished setting it up, and I now have a great video editing rig (well, aside from the *slow* hdd, but we'll deal with that next week), and I've started playing with some automated post-processing. Today, I'd like to show you [DeOldify](https://github.com/jantic/DeOldify). 

First, DeOldify is designed for still images, and it does a great job there most of the time. 

Have some still images: 

![Before]({{site.baseurl}}/images/17405-1-1329762897.png)
![After]({{site.baseurl}}/images/Enhanced_photo (3).jpg)

![Before]({{site.baseurl}}/images/himmelskibet-a-trip-to-mars-1918-holger-madsen-recensione-05.jpg)
![After]({{site.baseurl}}/images/Enhanced_photo.jpg)

![Before]({{site.baseurl}}/images/SPACE-PATROL-16.jpg)
![Enhanced_photo (1).jpg]({{site.baseurl}}/images/Enhanced_photo (1).jpg)

![Enhanced_photo (5).jpg]({{site.baseurl}}/images/Enhanced_photo (5).jpg)

There are better examples of the DeOldify github page, and on MyHeritage (which uses a new version of the same algorithms), but you get the idea. 

It works for video. Jantic posted some GIFs of video frames with some promising results. 

I decided to throw it at one of the worst videos in my collection, a low resolution, low contrast, noisy episode of Space Patrol. 

The original: 

<iframe src="https://archive.org/details/space-patrol-s-01e-01-low-480x-360p/Space+Patrol+S02e15+The+Phantom+Fleet+19520412+%5BLow%2C+480x360p%5D.mp4" width="640" height="480" frameborder="0" webkitallowfullscreen="true" mozallowfullscreen="true" allowfullscreen></iframe>

The color: 

<iframe src="https://archive.org/embed/sps02e15" width="640" height="480" frameborder="0" webkitallowfullscreen="true" mozallowfullscreen="true" allowfullscreen></iframe>

Some scenes from the colorized version look great! Some of them are flickery, messy, and ugly! There are lots of adjustments I can make on the front end to clean up the video and make it easier for deoldify to do it's work, and there are some tweaks I can do within DeOldify that might improve things too. 

So far, I'm tennatively hopeful. 

Have you done any video processing with ML? I'd love to hear about it. 
