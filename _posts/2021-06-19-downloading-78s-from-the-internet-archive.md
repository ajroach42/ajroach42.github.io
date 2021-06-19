---
layout: post
category: post
published: true
title: Downloading 78s from the Internet Archive
---
I'm leaving this as a note for myself, so that I can refer to it in the future, but it might help other people too. I'm downloading a large quantitiy of rips of 78 RPM records from the internet archive's [Great 78 Project](https://great78.archive.org/) ([for a project that I'll discuss later](https://mountaintown.fm)) and I want to ensure that I only get the "The preferred versions suggested by an audio engineer at George Blood, L.P. [which] have been copied to have [...] more friendly filenames." 

I'm using The [Internet Archive's python CLI](https://internetarchive.readthedocs.io/en/stable/internetarchive.html). It doesn't have an obvious method for doing this. It does, however, support searching files to download with a glob. This is how I've downloaded things like this in the past, but I've been doing too much bash and not enough Python recently, so I kept screwing up the syntax. 

The syntax to download friendly filename mp3s from the George Blood LP collection at the internet archive using the ia python tool is: 

```
./ia download --search="collection:georgeblood" --glob="[!_]*.mp3"

```

I kept trying `[^_]` which does not work because the ia client uses [Python's fnmatch function](https://docs.python.org/3/library/fnmatch.html) for a Unix filepattern match, as can be seen in [internetarchive client's code](https://github.com/jjjake/internetarchive/blob/f79ec26c5755294138fea3084b186a3f63d2b513/internetarchive/item.py#L554). 

So there we go, a one liner for the Internet Archive ia python CLI glob to ignore filenames with underscores.

(And that should be enough keywords that I actually find this in four years when I need to remember it again. :-) )
