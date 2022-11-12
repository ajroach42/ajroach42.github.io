---
layout: post
category: post
published: true
title: What Everyone Seems To Get Wrong About Mastodon (or What Mastodon't)
---
Let's get this out of the way up front. Twitter is a massive corporation that recently sold for tens of billions of dollars. Mastodon (or, really, the Fediverse) is an adhoc collection of dozens of servers run on spare change and passion by hobbyists the world over. 

## What Mastodon't

I'm sure you've seen, in the last day or four, the exodus of users from Twitter. Many of these users find themsleves reaching for the open source, federated "twitter alternative" Mastodon, or one of the several other Activity Pub compatible software packages. For me, and many other longtime denizens of the Fediverse, this has been a kind of mixed blessing. I've seen an influx of new followers, up 1,000 people or so in the last week. That's Significant, I have a wider reach now than I did before. It's also stressful, I have a wider reach now than I did before.

If you come to Mastodon expecting Twitter, you won't only be disappointed, you'll probably be angry. The fediverse is a great platform, it's where I spend most of my *social* time, and it has an awesome community. It's also a wierd niche project run by weird nerds, queer people, furries, neurodivergent people, tech people, anarchists, and radicals (I'll leave it up to you to figure out which of those apply to me.) 

We built this thing, some of us over the last 10 years. We built it to provide a place to do Social Media that wasn't owned and controlled by some behemoth that could be sold to Elon Musk. 

Guess what? It was a good idea. 

We built it, we're proud of it, some of us are defensive of it, some of us are lamenting the way that it is changing, and some of us are angry that All These New People won't just Use The Platform the way we want them to. This is normal, and we'll get over it (or we won't, and we'll leave.) One server admin who I've been following for years described it as [Mastodon's Home Invastion](https://www.hughrundle.net/home-invasion/). He makes some great points. 

I'm not here to address the new versus old, the Content Warning Debates, or any of the rest of that. I'm here to re-hash the same FUD that pops up every time Mastodon is in the news, and maybe one or two new fears. 

Most of this fear is bullshit, or at least misunderstood or misrepresented. The whispers of "Eternal Septemeber" are especially frustrating. I don't want to spill a lot of bits to re-hash the same arguments that have been made over and over again, but I do want to address a couple, and talk about what Mastodon is and isn't.

What the eff is The Fediverse?
------------------------------

So let's start from the top, what the eff is the Fediverse? The Fediverse is a different kind of social network. It started as implementation of the OStatus Protocol used by GNU/Social, and expanded to include ActivityPub when ActivityPub became a thing. OStatus support is mostly legacy or non-existent for most of the fediverse.

Mastodon is the largest, and most widely used software making up the Fediverse, but it's far from the only one. There's pixelfed (like instagram), peertube (like youtube), and a bunch of others. 

Mastodon is a platform for sharing 500 character messages (or longer, depending on the configuration of your server), these are colloquially known as Toots, in a timeline.

In theory, this is much the same as Twitter, and Mastodon has drawn lots of comparisons to twitter (even from me) but there are some big differences between mastodon and twitter that are worth discussing.

### 1) Mastodon is federated and decentralized

*   Okay, so what does that mean? It means that, unlike Facebook or Twitter where there is One place to interact with the service and that place is entirely controlled by a single corporation, with Mastodon there are dozens of different places you can interact with the service (known in this case as instances.)
*   Anyone can launch their own instance, and any instance can communicate with any other instance.
*   ( Well, mostly. We’ll discuss that more below. )
*   This is really cool! Because it means that no single company can own or control The Fediverse. No single company can shut us down. There is no Single Point of Failure.
*   This is also kind of dangerous, because it means that individual instances might not be trustworthy, or they might disapear without warning. Even long standing instances like venerable cybre.space are not immune to this. My own instance (retro.social) has experienced downtime that can be measured in days. I think this is okay, good even, but I might be in a minority there.

There’s a local timeline, showing all public posts on the local instance, and a federated timeline, showing all public posts that have been seen by users on this instance. On a small or medium sized server, the Local timeline is likely to turn in to a kind of town square. A place where people can get to know one another. On medium and large instances, the FTL becomes a firehose, moving so quickly that it is impossible to keep up. It does enable some discoverability and serendipity, which is Welcome because discoverability on The Fediverse is different (and probably more difficult) than on centralized social networks.

There is no single company in control. It's one big network, comprised of dozens of independent cells, many of which don't even interoperate with one another for safety or moderation reasons. There is no Spokesperson for Mastodon. There is no consensus. There are people, complicated and messy as ever. There are a lot of us, too. Instance Admins, I mean. Collectively, our moderation staff is probably the same size, or larger, that what is employed and deployed by the commercial platforms. But we're largely unpaid volunteers, doing this because we believe it should be done. 

### 2) Mastodon has good, but imperfect privacy controls

*   Individual users can choose on a per-post basis who to share their toots with.
*   Individual users can choose on a per-user basis to mute or block specific accounts
*   Instance administrators can choose on a per instance basis to mute instances (allowing users to interact between the instances, but preventing content from one instance from appearing in the federated timeline of the other instance) or block instances (especially useful when troll instances spring up.)

Some of these features depend on federating servers following the rules. Some federating servers do not follow the rules. There is room for abuse here, and bad actors do attempt to abuse this occasionally. (For the most part, at least so far, this has been inconsequential.)

There is no end to end encryption. Any expectation of privacy is a function of the software. This is true of commercial social networks as well (and we've already seen a breakdown in twitter's treatment of protected tweets, proving that they're struggling with this problem.) 

### 3) Mastodon does not have global usernames.

*   Right now, I’m @ajroach42@retro.social
*   You could be @ajroach42@mastodon.cloud, and confuse lots of people. I wish you wouldn't, but it's possible.
*   This is a feature, not a bug.
*   You can have multiple accounts on multiple instances, and you might want to (see point about instances disappearing above)
*   For example, you may choose to have an account on an instance that only federates with a select few other instances, so that you can talk in relative privacy (or a locked account, with follower only posting) and also have an account on a bigger instance, to keep up with the conversation on the federated timeline
*   You can export your following and follower lists, and import them to another account with ease, making account migration easy.
*   So if your instance dies, you can continue following all the people you followed before, as long as you prepair ahead of time
*   You can Verify your account somewhat simply, using a built in feature (a rel="me" link).

That user verification thing trips a lot of people up. The internet archive did it right, you can see their account at @internetarchive@mastodon.archive.org. Hard to impersonate that. 

### 4) Mastodon is open source, under the AGPL

*   This means you can make your own modifications to Mastodon
*   This means that your modifications have to be released under the AGPL
*   This means that anyone can contribute to Mastodon, and help the project grow
*   So if the service is missing a feature you’d like to see, implement it and make a pull request.

Glitch.soc was an early Mastodon fork with lots of additional features. Recently, Hometown has sprung up, and I'm a big fan of the hometown software. More will come. 

Additionally, Mastodon is built on open standards. You can interact with Mastodon without ever using Mastodon. (hence, the fediverse.) 

### 5) Mastodon works on iOS and Android

*   There are good clients available for both platforms, and I have enjoyed using it as a mobile application.
*   The website also works well in mobile browser. Most of the time, that's how I use it.

### 6) Most Mastodon instances take a hard line on harassment

*   This is a community project, and few instances currently have round-the-clock support
*   But the community policies of most instances explicitly forbid harassment, and I’ve seen this taken very seriously.
*   It’s not perfect, but it is in good faith, and it’s more than twitter ever did

### 7) Mastodon isn't a Twitter clone

*   This is way weirder and different than the social networks you’re used to.
*   It’s more like usenet, or even BBSs than a traditional social network
*   Adjust your expectations accordingly

### 8) Mastodon isn't one thing, the fediverse isn't one thing

We're dozens upon dozens, with different goals and desires and definitions of success. Some of us have been here for decades and some of us will still be here decades from now, and we're glad you're joining us for the time that we're together.

Addressing Concerns
-------------------

I've been a mastodon user for half a decade or more, and it has legitimately had a measurable, massive impact on my life and my wellbeing.

As new users flood in, I see the same complaints, concerns, and fears. I'd like to address some of them:

### What do I do if my instance dies?

Import your follows and followers to a new instance. It's easy and the tooling is robust.

Have fun. Back up your list of people you follow occasionally. Don’t worry about the social capital of identity. This is anti-capitalist software.

To be clear, many instances will die over the next few months.

There has been a rush of new instances in the last several days, and a lot of them won’t make it. Support your instance admin finacially if you can. Or host your own (single user) instance, and then you only have to worry about yourself.

### How do I prevent people from impersonating me?

Verify your identity against another website using a rel=me link.

If you have an official URL associated with your name, consider self hosting. 

Publish your prefered Mastodon handle and instance in multiple places, so that it’s easy to find. You can also use tools like The Mastodon Bridge to verify that you’re interacting with the people you think you are.

### I heard that instance admins can read your DMs

Yep, that’s true. It's not easy, it's not like there's a "Show me the DMs" button. But the text of the DMs is sitting unencrypted in a database, and if I was willing to put in the twenty minutes of work to parse that DB schema, I could probably find them. 

It’s also true for Twitter, for Facebook, and for Email (unless you’re using encryption), except that on those platforms there is a "Show Me The DMs" button, and dozens (hundreds?) of non-full-time-employee contractors have access to them at any given moment. 

Heck, Police don’t even need a warrant to access any electronic communications older than 6 months, thanks to a dumb law from 1986, and social services don’t have to notify you that your data has been accessed.

Gmail targets advertisements against your email and scans your photo uploads. People are already reading your DMs, and your mastodon admin probably isn't among them.

Don’t use a social network for publishing senstive information.

This is not a Mastodon specific problem. If you have something that needs to be shared actually in private, use strong encryption in the form of PGP, OTR, or a secure messaging app like Signal.

### What about bad actors on other instances? Or bad instances?

This is a real problem, sometimes. When it is a problem, talk to your instance Admin about blocking the bad instance. This is not a Mastodon specific problem, but Mastodon has better tools for fighting this problem than other platforms.

### But The Fediverse is doomed to die!

Nah. 

Mastodon started as an extension of the GNUSocial protocol. GNUSocial had been around for 10+ years. Lots of different software exists to support the fediverse, It’s not going anywhere. Use might wax and wane, but because it’s decentralized and federated, it can’t really die.

Heck, if anything, it’ll out live twitter.

### But it’s too complicated, it’ll never replace twitter!

Nope, it won’t replace twitter. It will provide an alternative to twitter for those folks that want one. And it’s fun!

Eternal September
-----------------

If you're not familiar with the phrase, "Eternal September" is a phrase used to reference the death of usenet. The legend goes: Every September, new students getting usenet access for the first time would be noisy and ignore existing norms and expectations. These new students would overwhelm the network, rendering it an unpleasant place to be for several weeks, then they'd figure it out and calm down and things would go back to normal. Lather, Rinse, etc.

Then enter AOL.

AOL gave Usenet access to their users. Usenet was flooded with lots of people who had no interest in the existing culture of usenet. It floundered and sputtered out.

That's how the story is normally told anyway. "Eternal September" has come to mean "New people are here, and I don't like it." I have my doubts that the story was that simple, but I wasn't there. I am here, though, on the fediverse, and I'm sick of hearing people whisper about an eternal september.

Let me say explicitly: The Eternal September mindset is both harmful and backwards. It's gatekeeping. Banish it from your mind. Embrace the chaos, help people find a place to fit in. Or don't, ignore them. This isn't usenet, this is the fediverse. It doesn't have the same weaknesses usenet did, it isn't an easy vector for Spam, the moderation tools are better, the federation tools are better.

Twitter's meltdown is not AOL.

[Activity Pub on Wikipedia](gemini://wikipedia.geminet.org/en/ActivityPub)

[Explaination of Mastodon's identity verification](https://docs.joinmastodon.org/user/profile/)

[My Mastodon Instance](https://retro.social)

[No More Eternal Septembers](https://tedium.co/2020/10/13/eternal-september-modern-impact/)

What Everyone Seems To Get Wrong About Mastodon was originally published on 2022-11-06 at [gemini://gem.ajroach42.com](gemini://gem.ajroach42.com) - This web version has undergone minor revisions.
