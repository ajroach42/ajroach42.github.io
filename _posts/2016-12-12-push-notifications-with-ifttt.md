---
layout: post
category: post
published: false
title: Push Notifications with IFTTT
---
Apparently [IFTTT](https://ifttt.com/discover) can monitor RSS/ATOM streams ([like mine](http://ajroach42.github.io/feed.xml)) and perform an action for new items. That means that I can have [TradeSocial](http://ajroach42.github.io/tech-meets-diy-punk/) output an RSS feed for the system as a whole, for the feeds of individual users, and for @replies. Then I can tell IFTTT to look at those feeds and [send and email|send a push notification|Post a Tweet|etc.] any time one of them changes. 

That adds iOS/Android notification, email notifications, twitter notifications, and all kinds of other goodies to [OfManyTrades](http://ofmanytrades.com) with *very* little coding on my part, which is awesome. On the other hand, it relies on a (closed source) third party, which isn't cool. Since the heavy lifting is done with RSS/ATOM feeds, though, a community alternative can be spun up without any changes to the TradeSocial software (and it can live along side the IFTTT solution!) 

I love open standards, and simple solutions. 

(This post is a test post for this feature.) 