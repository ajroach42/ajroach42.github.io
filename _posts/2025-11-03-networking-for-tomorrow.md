---
layout: post
category: post
title: Networking for Tomorrow
---
I've been thinking ([and that's not good for anyone, and everyone should be holding their breath](https://communitymedia.video/w/exFoSTiCszM2r52Qsi1sdy)) about technology again. I can't help myself; every time I think I'm out, they pull me back in. Mostly, I'm thinking about technology right now because I'm contemplating the ways that the US is a failed state, and thinking about the kinds of technology that we're going to need to get through to whatever comes next. This is mostly a post about technology, but the next header is a justification of my claim that the US is a failed state. If that might be too much for you to read right now, skip it.

## The current state of the US:

It feels like the last 10 months have been an unending onslaught of horrible actions, the erosion of human rights, and the destruction of the social fabric that has held society together, but it's not the last 10 months, it's the last 20+ years. Things just unwind faster at the end.

Put simply: The gutting of the Fairness Doctrine and the 1996 Telecommunications Act enabled the rise of massive, right-wing media conglomerates like Sinclair Broadcast Group and iHeartMedia (formerly Clear Channel). This systematically eliminated local, independent journalism and created a national propaganda apparatus that could broadcast centralized, partisan talking points through hundreds of local affiliate stations, masquerading as local news. This hit small towns especially hard and led to a massive radicalization of rural communities.

This is Extremely Dangerous to Our Democracy.

<iframe title="This is Extremely Dangerous to Our Democracy" width="560" height="315" src="https://communitymedia.video/videos/embed/kJ3dojouKA3G5onEaKq1Vu" frameborder="0" allowfullscreen="" sandbox="allow-same-origin allow-scripts allow-popups allow-forms"></iframe>

Between the DMCA, the Patriot Act, the founding of ICE, and the passage of *Citizens United*, we laid the groundwork for oligarchic authoritarianism in the US. In the years that followed, we watched a slow slide in that direction, which has only continued to accelerate as the remaining checks on power are removed, leading to the situation we have today.

On top of our rightward drift, we are flirting with a massive economic recession, and any number of things could send us tumbling to levels of poverty that are **unprecedented**. [Regional banks are already looking **shaky**](https://finance.yahoo.com/news/live/stock-market-today-dow-drops-300-points-sp-500-nasdaq-slide-as-regional-bank-woes-hit-markets-133458076.html), and there is an **apparent** liquidity crisis. A large portion of the current stock market appears to be tied up in a bubble built around [nearly **fraudulent** **accounting** in AI firms.](https://pluralistic.net/2025/09/27/econopocalypse/)

All the while, we're also cutting funding for programs that help people in poverty, stripping people of healthcare coverage, destroying our supply chains, and shutting down the government if anyone tries to stop us.

Federal agents, at the direction of the president and in defiance of court orders, are kidnapping people out of their homes (or at the courthouse, or at work) and putting them in concentration camps or making them disappear without a trial. [County sheriffs are putting people in jail for posting to Facebook.](https://www.usatoday.com/story/news/2025/10/29/larry-bushart-arrest-charlie-kirk-memes-charges-dropped/86970944007/)

[City workers in GA ran a man over with a bulldozer and then tried to cover it up](https://www.youtube.com/watch?v=hywVaznsHIs). Months before that, [they shot an unarmed man who was sitting on the ground in the forest and then lied about it extensively](https://en.wikipedia.org/wiki/Killing_of_Tortuguita).

The courts are trying to put some limitations and constraints on these "law enforcement" actions, but the agents in question are [actively and flagrantly ignoring those court orders](https://www.independent.co.uk/news/world/americas/us-politics/trump-federal-court-ruling-ignore-b2792939.html), and when there is a financial penalty levied against law enforcement, it is almost always paid out of the pockets of people in their communities, not the officers themselves.

People are being murdered in the streets (by cops, by other people) for crimes such as [*insufficient respect for the military*](https://www.nbcnews.com/news/us-news/flipped-middle-finger-war-memorial-was-shot-dead-rcna228826) or *being homeless* or *legally possessing a firearm* or *going to a concert* or *being a trans person*.

I don't want to be alarmist. I'm trying to present an accurate picture of the US as it exists today. It is alarming. What happens next is hard to predict, but it seems the [dominoes are falling](https://www.reuters.com/business/feds-standing-repo-facility-hits-record-high-policy-meeting-outcome-looms-2025-10-29/).

My guess is that we're less than 18 months away from a major, global financial crisis and that we're ill-equipped to weather it without significant political change.

*Things will never go back to how they were before. Before was an anomaly. We have to build something new.*

## Why does this make you think of technology?

The thing that I want out of my computers and other technology, mostly, is to connect me with other people. [Community Software](https://ajroach42.com/community-software-building-the-future-inside-the-rotting-husk-of-the-past/), written by people for other people, an explicit rejection of the advertising panopticon that serves mostly to widen our current social divides and push people further into extremism.

In a world where we can't trust the rule of law, where the internet is under constant attack, and where poverty is likely to reach **unprecedented** levels, it becomes increasingly important that we have ways to connect with one another that aren't dependent on the whims of governments or **corporations**, and aren't being monitored 24 hours a day.

### Revisiting the BBS
This is an idea that I've batted around a lot over the years. I've run some **experiments**, including a deployment in Kennesaw in 2015 and another in the DC metro in 2019. The concept is sound, the hardware is abundant, and the low-level software is all in place. All we have to worry about is the userland.

I think about this every few years ([2016](https://ajroach42.com/a-modern-bbs/) or [later 2016](https://github.com/ajroach42/Docs/blob/master/TorBBS.md) or [2017](https://ajroach42.com/steps-towards-a-web-without-the-internet/) or [2019](https://ajroach42.com/tech-for-the-future/)). I tend to tinker with it a bit in private, get excited about it, write a blog post or two, keep tinkering, get distracted, and move on to something else.

But it's been a decade since my first **experimentation** with a modern BBS, and I've learned a lot. I've watched some projects grow and progress and others fizzle and die, and through that, I think I've learned enough to propose something new, or at least to refine what I've done in the past into a coherent proposal.

### The Vision: A Network of Neighborhood Nets

Imagine a city where every apartment building, community center, and local cafe hosts a small mBBS node. You connect your phone to the local node to read community announcements, argue about local politics, or share music from local bands.

When you leave, your phone automatically syncs the latest messages. As you move through the city, your phone becomes a "carrier pigeon," silently exchanging these messages with other nodes you pass, or with your home node later that evening. A message from the east side can slowly make its way to the west side, hop-by-hop, through the devices of ordinary people, creating a true people-powered network.

The mBBS project seeks to revive the ethos of early BBS culture by creating a standard for local, distributed, and community-operated social networks using modern technology. It is designed to be a censorship-resistant, surveillance-proof communication platform that operates as a parallel, offline-capable network.

The core philosophy emphasizes low-cost, high-participation, and ease of use, treating nodes as disposable “cattle, not pets.” The project aims to provide a set of guidelines and a reference implementation, with the explicit goal of fostering a multi-vendor ecosystem of compatible servers and clients, analogous to the interoperability seen in historical networks like FidoNet.

### The Plan

I'm working on a specification for a message format that is text-based, with optional key-based encryption and signed hashes from the originating user and the transmitting server, and a reference implementation for a client, a server, and support for multiple transfer/sync methods, including LAN, LoRa, VPN, and full sneakernet.

The system synchronizes content asynchronously across a federated mesh. The project encourages a diverse ecosystem of compatible servers and clients, much like historical networks such as FidoNet, fostering a community-driven approach to building local digital commons.

### Core Goals

*   **Open Protocol and Ecosystem:** The project defines a standard method for node-to-node and client-to-node communication. While a reference implementation will be provided, other server and client implementations are explicitly encouraged to promote widespread adoption and innovation.
*   **Infrastructure Independence:** Operate outside the conventional internet, using RF protocols like Wi-Fi or LoRa, but also sneakernet file transfer.
*   **Accessibility and Low Cost:** We're targeting low-power computers, SBCs, embedded devices, and other machines that were destined for the landfill.
*   **Ease of Use:** It must be easy to discover, to use, and to deploy for end-users and server operators.
*   **Offline-first, Federated, Asynchronous, and Delay Tolerant:** The core of the project is a local message board that will sync with other boards via store-and-forward, not requiring constant connectivity.
*   **Optional message signing (authentication) and encryption (privacy).**

This is Community Software. It is a [Small Thing](https://ajroach42.com/the-small-things-manifesto/). It is intended to be People First and ultimately to do very little. Pass messages, store and forward, verify where they came from when that's appropriate, and where they're going when that's appropriate.

That's it.

### Non-Goals and Explicit Exclusions
*   **No Blockchain/DLT:** The system will not use a distributed ledger or cryptocurrency.
*   **No Eventual Consistency Promise:** The network is asynchronous and best-effort.
*   **No Complex Trustless Fabric:** The design acknowledges a base level of trust and uses simple blocking tools rather than attempting to algorithmically purge all malicious actors.
*   **No Monopoly:** The project is a standard and a reference, not a single, closed implementation. Interoperability is a primary objective.

### Current state
I have a design doc and a working draft specification for the client and server API, and I have a rough prototype running on a cheap SBC at our cafe and another one running in my home.

mBBS currently supports manually initiated sneakernet sync and manually initiated LAN/VPN server-to-server sync only.

It does support message signing and message **encryption**, but not in a way that I think is particularly worthwhile. Everything about this exists as a proof of concept, not as something ready for general consumption.

### Next steps.
This week, I'm going to add a naive implementation for automatic sync on LAN between servers. Then I'm going to document how I built and configured the existing servers and post instructions for running one yourself, along with the existing software stack.

There is not currently any client software beyond a simple web app. Building a prototype desktop app and PWA will be the next development milestone.

Then it's implementing automatic server > client > server sync (carrier pigeoning).

In parallel, I'd like to get a few more servers online to begin testing hop distance.

I'll post here again when it's ready, so subscribe via RSS or follow me on the fediverse for that announcement. This is pre-alpha, bare minimum. It might never move far beyond that, but if I can get some people on board to work with me, it might go a little further.