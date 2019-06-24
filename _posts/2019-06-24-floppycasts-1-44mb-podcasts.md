---
layout: post
category: post
published: false
title: 'Floppycasts - 1.44MB Podcasts '
---
I've been working on making podcasts and videos about old movies, and old computers, and bigfoot hunters, and people living on asteroids in outerspace, and the crew of a spaceship, and masked heroes who cut promos on one another pro-writing style. It's fun! It's time consuming! I have lots of half finished stuff sitting around that I've slowly been editing and prepping for release, and that's got me thinking about releasing podcasts on floppy disks. 

I've been talking about #floppycasts on the fediverse as I experiment with different codecs and quality settings, and I wanted to collect some of those thoughts in to something a little more coherent than slapdash microblogging. So this is that! 

I've run in audiophile circles for years. I sold records and hi-fi gear at a shop that carried single pieces of audio gear that cost more than $40,000. Later I dabbled in what can only really be described as mid-fi. Stuff that sounds good, enough, and sounds great for the price. In doing so, I learned a lot about the way hearing works, and a fair amount about personal preference and individual tollerance. 

So, this weekend, I decided to take all of that accumulated knowledge and use it to compress roughly half an hour of speach down to a size small enough that it will fit on a floppy disk (with bonus points if it would then be playable on a machine that would have originally shipped with a floppy drive!) 

## Codecs 

I tried a lot of codecs! Here is a short list of some of the codecs I tried, and the smallest size I was able to get out of them for 30 minutes of speech that was still inteligable: 

- Speex: 3MB 
- Ogg/Opus: 1.2 MB 
- MP3: 1.5 MB 
- Ogg/Vorbis: 3MB 
- AAC: 7MB 

Now I was performing these transcodes from a wav file that I had processed in audacity as I will describe below. I used lame, libopus, and ffmpeg for conversions, and likely would have been able to get smaller sizes from Speex and AAC if there were more options I could tune in the transcoders. 

Put another way, while Opus actually sounds pretty okay at 1.2MB, the only reason I was able to get it that small is because opusenc gives you a *lot* of freedom when your encoding, and provides that freedom through a really easy to understand CLI. Similarly, with the mp3 encoder I was using, it was possibel to carefully fine tune the files for very small file size. 

The same was not true about the other codecs listed, and the resulting files are the result of tuning each setting to the loewst quality option it would allow. I presume that, if I was given more control over the encoding process, I could produce smaller files out of the remaining codecs, but I don't think that matters much (as you'll see below.) 

## Method

First, I grabbed a half hour sample in wav format from Archive.org's OTR selection. Second, I opened that wav file in audacity and performed the following alterations: 1) mixdown to mono 2) resample down to 8KHz, 3) save as an 8-bit wav file. 

This results in a wav file that is surprisingly small, while still sounding ... I mean, not great, but better than you'd expect. 

Then I encoding the resulting wav file with opus at between 6 and 10 average Kbps, variable bitrate, tuned for speech. This results in a file under 2MB in size each time, and in my experiments an average bitrate of 7 resulted in a file under 1.44MB from multiple samples, with audio quality that was honestly and truely awful, but really no worse than AM radio. 

I also encoded the same wav file as an MP3, forcing mono, in CBR, at 8kbps. Anything lower than 8 is not allowed by my encoder. VBR resulted in larger files than CBR at this bitrate in my experiements. This resulted in a file that sounded worse than the Opus file, and that was a little larger. When I say "worse" here, I mostly mean that a large amount of clarity disapeared from the file. It was still possible to make out all the words, but every ounce of sharpness had been sucked away. Like the beginnigs of a tape loop. 

Unfortunately, MP3s need a length of ~22 minutes to fit on a floppy disk, as opposed to the 30+ minutes achievable with opus. 

## Playback 

The Opus files will play back on Windows 98 and newer, on Pentium MMX and newer processors using Winamp version 2.5 and the [OPUS plugin](http://forums.shoutcast.com/showthread.php?t=452974), or on very fast Pentium (and possibly even 486) processors in DOS using [Mpxplay](http://mpxplay.sourceforge.net/) and the OPUS plugin. 

(I did have some trouble with the most recent version of the winamp opus plugin on my Windows 98 install, and was only able to get it working on windows 98SE. Earlier versions would open on Windows 98. If at first you don't suceed, etc. etc.) 

I was unable to get the OPUS file to play back in any other programs on either OS, and I was never able to get the OPUS file to play back on anything in my collection slower than a Pentium MMX (although it has been suggested that a high end Pentium, or possibly even a very fast 486 should be able to handle it, I don't currently have rigs available for testing.) 

The mp3 file will play back in the same programs (without plugins) on each OS, and has been verified working on a 486 DX 100 with a Sound Blaster AWE32 (I think?), and on a 70 MHz Pentium laptop with a Sound Blaster Pro. I suspect that it will also play back on slower 486s that would otherwise strugle with mp3 sound reproduction as a result of the incredibly low bit-rate, but I have been unable to verify that so far (as I don't have compatible soundcards in any of my older 486s) 


## Results 

I... I guess I have a viable method for putting podcasts on floppy disks? I'm going to stick with mp3 for now, because of the wide variety of playback options, but if I end up actually attempting to distribute floppycasts, I'll probably make OPUS an option in the ordering system. 

I don't currently have any playback examples posted anywhere, or any files available to download (as I wasn't working on my own files) but I'll post some short samples in the near future. 