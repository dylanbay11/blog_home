---
layout: post
title:  "Over 400 Free PC Games - Data Collection"
date: 2024-03-28
fontsize: 24
description: "Giving away a game a week for five years is a lot."
image: "/assets/img/egs_dark.jpeg" 
# image grabbed from https://store.epicgames.com/en-US/news/the-holiday-sale-returns-on-december-17-plus-15-free-games
# publish: false
# hide: true
---

If you've ever played a video game on a computer, chances are you've used or heard of Steam. Launched in 2003 to distribute game studio Valve's own games, but later expanded to become a storefront for video games from third party developers, Steam became so wildly successful that today Valve practically gave up making its own games. Steam became so dominant in the space by the mid-2010s that even a few major studios splitting off and making their own launchers hardly seemed to matter, and in recent years some of those same studios (EA, for example) have come back to Steam, because that's where the money is. In 2013, for example, [one source](https://www.bloomberg.com/news/articles/2013-11-04/valve-lines-up-console-partners-in-challenge-to-microsoft-sony) had Steam pegged at a whopping 75% market share. 

[Statistia](https://www.statista.com/topics/4282/steam/#topicOverview) estimates that even today Steam remains a behemoth, with over 10,000 new games in a single year and peaking at 10 billion dollars in revenue! The path to this windfall: taking a 30% cut from every sale on the platform, making Valve the ultimate PC gaming middle man. Cue a challenge. Epic, both maker of popular game engines that power game graphics and physics, and publisher of smash 2017 hit Fortnite (itself estimated to have brought in [20 billion](https://www.tweaktown.com/news/94476/fortnite-made-over-20-billion-in-revenue/index.html) dollars in lifetime revenue), decided to follow a similar path, and expanded their own launcher to sell third-party games. The pitch? [Only a 12%](https://www.gameinformer.com/2018/12/04/tim-sweeney-answers-questions-about-the-new-epic-games-store) cut for Epic. At the end of 2018, this expanded storefront went live. 

**The problem?** Change was great for developers, but many users had racked up tons of games and didn't really care to switch. But what DO gamers quite like? **Free stuff.**

As an incentive to pick up and get locked into the platform and corresponding game launcher, Epic started partnering with all kinds of game developers (offering them usually a lump payout) to offer free games for limited times on the storefront. They started out with a bang, giving away popular indie game Subnautica, and then every two weeks came out with something new. This actually accelerated, and in June 2019 they upped this to a game every week... and sometimes two! Astonishingly, this continues to this day, making over five years of giveaways. Occasionally, a game is given away again months or years later, but other games are completely new. Across this time period, there have been over 400 giveaways!

Clearly, this is a lot of games, and something I felt would be very interesting to look at. Some of these were big games, too. Grand Theft Auto V was given away, brought over [7 million](https://www.theverge.com/2021/8/19/22631952/epic-games-store-gta-v-free-game-7-million-new-users-apple-trial) new users, and crashed Epic's servers by itself, for example. 

<figure>
	<img src="{{site.url}}/{{site.baseurl}}/assets/img/TopReddit.png" alt=""> 
	<figcaption>The most-hyped games given away according to reddit posts in a subreddit for gaming deals</figcaption>
</figure>

#### Collecting some data

Thankfully, I'm not the only one interested in these games. For my data collection, I noticed that there was a nicely formatted list found [here](https://www.steamgifts.com/discussion/S4e2c/free-epic-games-store-list-of-all-weekly-free-games-every-thursday-at-11-am-et). Others have looked into repeat games, but there's a lot of other information that I haven't seen anyone else look into. For example, what kinds of genres? How many different developers/publishers worked with Epic? How many dollars worth of games were given away? What kind of ratings were the games given, are they all well-reviewed hits or is the list full of shovelware?

Examining *how* I collected this data, I hope, can be helpful to others in a similar situation who want to take another step, and acquire and analyze their own data for a similar kind of question. 

I should state that there are about a half dozen lists floating around by various websites and users with about the same amount of data, probably in turn scraped from Epic's homepage or news sources. I chose this list in particular because it also offered links to each store page, which I felt could be very helpful. However, other than name and date, the list isn't very populated. My first step was to simply get this data myself, in a good format. Web scraping to the rescue!

<!-- If you're seeing this post, you're ahead of the curve! Stay tuned for the next update, on a project to collect data about Epic's five-year free game giveaway experiment of over 400 games via web scraping and APIs. -->

<!-- Intro about Steam's dominance, a chart about that dominance

(also: Potential data or charts from various Epic Game Store Year in Review posts, aggregated?)

Story about EGS free games and their efforts, including biggest giveaways

Get down to brass tacks: explain initial list scraping and desire for more data

Problems faced trying to scrape links themselves

Solution (mostly): use wrapper for API (how much detail??), focus on thought process I think

(Optional) Problems faced with age restrictions, empty rows

Conclusion, hype for follow-up data, desire to fill in empty bits (Selenium?) -->