---
layout: post
category: post
published: true
title: Tiny Music from the American Public Domain
---
Thanks to the (inadequate) [Music Modernization Act](https://en.wikipedia.org/wiki/Music_Modernization_Act), audio recordings entered the [public domain in the US](http://ajroach42.com/public-domain-day-2022/) for the first time this year. I've been celebrating this in various ways, and one of those ways is making copies of these songs that are Tiny and can be distributed Anywhere. 

This is not Archival work. This is leveraging Archival work to make some this music more accessible, to make it universally available. 


## Kid Ory's Creole Trombone 

<audio controls>
  <source src="http://ajroach42.com/images/Ory-Trombone.ogx" type="audio/ogg">
  Your browser does not support the audio element.
</audio>
[Download](http://ajroach42.com/images/Ory-Trombone.ogx) - 413 KB 

Here's Kid Ory's Creole Trombone as a 413KB, 16Kbps opus file. 

The "original" that I used to make this was digitized from a pirated press released in the early 20s of an impossibly rare jazz side. It has been called the *first* Jazz recording. It probably isn't that, but it is the first recording of a Black Jazz band from New Orleans. 

And it was wildly popular! It was popular enough to be pirated. But it was also super controversial, and frequently destroyed. Originals are basically impossible to find, so piracy paved the way for preservation. 

Now it's in the public domain in the United States, and I've compressed it down small enough that you could put two or three of them on a single floppy disk. 

I've made it small enough that it can be transmitted by basically any means. 

It would take a little under 3 hours to transmit this over a standard hayes modem. 

22 minutes to transfer at 2400 baud.

Faster than real time on standard 56k dial-up. (a little under 1 minute!) 

This is data representing music that can be converted in to sound representing data (representing music), and transmitted as sound representing data faster than it could be listened to as music. That boggles my mind. 

## Mamie Smith and her Jazz Hounds - Crazy Blues

Mamie Smith was the first Black woman in this country to sell a million records. She did that for the Okeh record label in 1920 with the song Crazy Blues. It, like Ory's Creole Trombone above, is now in the public domain in the US. It's a banger. 

![mamie-smith.jpg]({{site.baseurl}}/images/mamie-smith.jpg)

The above photo of Mamie and her band is 773KB. That's already pretty impressively small for a picture that big and clear. 

<audio controls>
  <source src="http://ajroach42.com/images/mamie-blues.oga" type="audio/ogg">
  Your browser does not support the audio element.
</audio>
[Download](http://ajroach42.com/images/mamie-blues.oga) - 395 KB 

But the song above is 395K. Less than half the size of the photo. 

Is it perfect? No. Is it archival quality? No! But Preservation = Future Access, and it's damn accessible, and it sounds good enough. It is Small enough that you might have hundreds or thousands of copies before you noticed. It's representative of the music, good enough for listening, and small enough to be endlessly duplicated. 

If you need an archival quality copy, [archive.org has an 80MB FLAC](https://archive.org/details/78_crazy-blues_mamie-smith-and-her-jazz-hounds-perry-bradford_gbia0076149a) file of a different physical copy of the same recording that definitely contains more data than this, and sounds significanlty different, but uhhh.... 

Look, more than 200 of this file fit in the same storage space as one 80MB FLAC file. Yes, the FLAC file is lossless, it's a perfect representation of the music that was originally recorded. The Opus file I'm embedding here is Lossy as hell. It's like comparing JPGs to TIFFs, or xerox copies to photographic prints. 

Except that these JPGs, these xerox copies, are so overwhelmingly miniscule that I can fit hundreds of songs in the same amount of disc space that would normally hold 1 lossless file. 

I know, I'm rambling, but I'm impressed. 

## W.C. Handy - St. Louis Blues

Here's another very early Blues song. This is a track written in 1914 by W.C. Handy. I'm not certain when this recording was made, but the record it was pressed on dates to the 1940s. That means that this song is in the public domain, but this recording might still be under copyright, depending on when it was originally published. 

Handy recorded this song several times, and some of those recordings are certainly in the public domain. 

Lots of other people also recorded this song, and many of those recordings are also in the public domain. 

<audio controls>
  <source src="http://ajroach42.com/images/handy-blues.opus.ogx" type="audio/ogg">
  Your browser does not support the audio element.
</audio>
[Download](http://ajroach42.com/images/handy-blues.opus.ogx) - 206 KB 

Thanks to some tips from [Thamesynne on the Fediverse](https://dragon.style/@thamesynne) I was able to push this one even smaller than the others without any glaring faults in quality. It honstly sounds pretty good, and it's 10Kbps. 

10 Kilobits per second. 

A standard 56k modem could recieve 5 copies of this song in real time. Could download this song in 1/5 of real time. 

## DIY 

Anyway, that's enough gushing. I'm doing this work with opusenc from wav and flac files using the following paramaters: 

```

 opusenc --bitrate 16 --music --downmix-mono input.wav output.opus

```

or from ffmpeg using the following paramaters: 

```
ffmpeg -i input.flac -c:a libopus -b:a 16k -map_channel 0.0.0 output.opus

```

Each of those commands crushes a file to joint mono, and re-encodes it as a 16kbps Opus file. You could tweak the 16 above up or down to get more fidelity or a smaller file.

If you're working with acoustically recorded 78RPM records, as I am here, it might make sense to downsample to a max frequency of roughly 8Khz, because acoustically recorded 78RPM records had a relitively limited frequency response anyway, and a lot of the sounds outside of that range are going to be surface noise introduced by the playback mechanism, and by decades of wear. 

But this isn't a hard rule, and it's a nuanced thing. The settings I described above are somewhat universal. For mono source files, these settings will get you a very small, reasonably good compressed file. If you start cutting frequencies out, you might get a smaller file (or you might not!) and you might get a better sounding file (but you often won't!).

A lot of the files here are 12Kbps or even 10Kbps. 10 is the lowest I've gotten Music to sound like Music. I have gotten spoken word all the way down to 6 without it becoming uninteligable. It's possible to go lower for speech in other codecs, but those codecs are basically useless for music. Maybe I'll talk about that some time. 