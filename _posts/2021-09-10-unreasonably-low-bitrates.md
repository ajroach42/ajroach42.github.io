---
layout: post
category: post
published: true
title: 'Unreasonably Low Bitrates '
---
I've been playing with encoding videos at very low bitrates. My entry in the Small File Media Festival won Lowest Bitrate, clocking in at around 30Kbps. You can [see it here on archive.org](https://archive.org/details/expedition-sasquatch-small-file-media-festival-submission) as an MKV with h265 video and ogg/opus audio. It was fun, but I thought we could do better. 

At the moment, I'm working on an original sitcom with some of my comrades from the [Maker Space](https://ellijaymakerspace.org). We just finished our teaser trailer, and this seemed like a perfect opportunity to really just destroy a video. 

So here are some examples. [[cw for strong language]]

# 720p - 512KB, ~60Kbps

<video src="https://retro.social/system/media_attachments/files/106/910/306/920/699/907/original/9776dfa6a3351f92.mp4" poster="https://retro.social/system/media_attachments/files/106/910/306/920/699/907/small/9776dfa6a3351f92.png" controls volume="1"></video>

# 240p 212KB, ~25Kbps 

<video src="https://retro.social/system/media_attachments/files/106/910/422/627/777/710/original/0cb5d594010a8079.mp4" poster="https://retro.social/system/media_attachments/files/106/910/422/627/777/710/small/0cb5d594010a8079.png" controls volume="1" height="480"></video>

The end results aren't exactly good, but they are pretty remarkable. 

For comparison, the average size of photos from my new phone is 7.8 MB. 

![IMG_20210903_162503994.jpg]({{site.baseurl}}/images/IMG_20210903_162503994.jpg)


I could fit 15 or 16 minutes of 720p video in the same space, or about half an hour's worth 240p. In the bandwidth it takes to transfer that photo, we could instead transfer half an hour of (barely) watchable video, or 15 minutes of stuff that's almost enjoyable.

I'm going to keep poking at this, as I'm fairly certain I should be able to get a 480p video down under 50 Kbps without making it entirely unwatchable. 


This is AV1 video, encoded with ffmpeg with the following settings:
```ffmpeg -i input-file.mp4 -c:v libaom-av1 -strict -2 -threads 16 -cpu-used 8 -filter:v fps=12,scale=720:-1 -crf 52 -c:a libopus -b:a 10k -ac 1 outputfile.webm```

Which results in very small videos with opus audio, and a max of 12 frames per second.
