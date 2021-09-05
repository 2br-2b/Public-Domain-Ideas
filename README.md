# Public Domain Ideas

A lot of the time, I have random ideas that could be really good projects, but which I don't want to or have the time to work on. This is a list of some of those ideas. I may or may not work on some of these in the future, but feel free to use them yourself!

While I'd like credit if one of these inspires you, no credit is necessary.

Also, if you end up using one of these ideas, if you open an issue or a discussion, I'd love to link to it! Open an issue and let me know about it!

Visit the [Discussions tab](https://github.com/2br-2b/Public-Domain-Ideas/discussions) to comment on a specific idea.

# Ideas

## Programs

### Anbox F-droid integration

[Anbox](https://anbox.io/) is a way to run Android apps on Linux. Could you make a CLI for [F-droid](https://f-droid.org/), then allow a user to install Android apps to Anbox with a command? Maybe make a package manager interface for F-droid on Linux?

Perhaps https://github.com/mvdan/fdroidcl could be used as a starting point to build this.

You could also use the EFF's new [apkeep](https://www.eff.org/deeplinks/2021/09/introducing-apkeep-eff-threat-labs-new-apk-downloader) to get apps from the Google Play Store as well.

This was inspired by Microsoft's adding of Android apps to their store.

### Anytube Video Platform Aggregator

There needs to be more competition in the video platform market. Youtube is the only major player, and startups like [Odysee](https://odysee.com/) and [Peertube](https://joinpeertube.org/) are struggling to catch up. One of the main reasons for this is that no one wants to watch some content on Youtube, then to switch to Odysee, then Dtube, and so on for all their videos. While I follow my creators via RSS feeds across platforms, this isn't easy for a non-tech-savvy user. Also, while solutions like Youtube-dl work, Youtube-dl violates [Youtube's terms of service](https://www.youtube.com/static?template=terms), which could lead to your Google/Gmail account being blocked.

My solution is to combine all of these platforms into one. In order to not violate the platforms' terms and conditions, you use embeds from the websites to display the videos on Anytube. The video links can be retrieved via rss feeds or apis, and many of the embeds for different platforms have the same format:

Youtube: 
```html
<iframe width="560" height="315" src="https://www.youtube.com/embed/pPmo21gkETU" title="YouTube video player" frameborder="0" allowfullscreen></iframe>
```

Odysee:
```html
<iframe id="lbry-iframe" width="560" height="315" src="https://odysee.com/$/embed/If-Video-Platforms-Were-Honest/8f64292ddd2303de5c4ee0908ddd5b0a276f4055?r=EBe4V7K8Gna5FwdqWkr3FzyLA6VhEbjW" allowfullscreen></iframe>
```

Peertube:

```html
<iframe width="560" height="315" sandbox="allow-same-origin allow-scripts allow-popups" title="ZOOM is becoming popular, but don&#39;t fall for the memes!" src="https://videos.lukesmith.xyz/videos/embed/dab28f3b-6026-4fd1-8b5a-8ffbb4c9cde3" frameborder="0" allowfullscreen></iframe>
```

Platforms to hopefully add:
- Youtube
- Vimeo
- Odysee
- Peertube
- Bitchute
- Rumble
- DailyMotion
- All the platforms!

### Sync application dictionaries

(I assume this is the same for Windows, though I can't confirm)

When I add a word to my personal spelling dictionary in LibreOffice on Linux, I expect the computer to now recognize the word everywhere. However, if I type that word in Marktext or Joplin later, I'll have to mark down every time that the word exists! It'd be nice if all the dictionaries were synced together.

### Signal gif search

Signal has a great interface for searching for gifs. The only problem is that the interface is buried away. If I want to find a gif and use it in another app, I need to send a message with the gif to myself, then copy it.

It'd be great if the search were lifted from Signal's code and made available as a stand-alone app. It could still be integrated with Signal, but I'd like it separate also for use in other apps!

### IRL Achievements

You get achievements for doing things in video games, but doing things IRL can be boring. People are willing to play Power Washer Simulator, but they aren't willing to go out and power wash in real life. Sometimes, you need the satisfaction of seeing meaningless numbers go up on a computer screen in order to motivate you to do things.

What if there was an achievement board for achievements in real life? For example, you could get achievements for going camping, going to college, going to trade school, going on your first date, getting your first job, getting married, staying single for long enough, or anything else!

You could monetize the product by having sponsored achievements: visit Disneyland, take a picture of yourself in a Spiderman costume, etc.

You could also have random achievements, like talk to a random stranger, play piano in public, etc. to help spice up life. The possibilities are endless!

[Habitica](https://habitica.com/static/home) has something similar to this, but IRL Achievements would be for doing specific things. You could have a global leaderboard to say who has the most IRL points, see what percentage of people have done XYZ, and use this to motivate yourself.


## Experiments to run

### GPT-3 Textbooks

What if you trained GPT-3 on logic textbooks? Could you somehow make the GPT model output valid logical syllogisms, or would you only end up with technical-sounding gibberish? You could get a lot of public domain books from [Project Gutenberg](https://gutenberg.org/), so it wouldn't be too hard to get a sample set.

What about if you trained GPT on Chemistry textbooks? Could it tell you any real facts?

What about other subjects?

## Religion

### Muzei saints wallpaper

It would be nice if there was a plugin for [Muzei](https://muzei.co/), an Android app to deal with live wallpapers, which changed the wallpaper to the saint of the day or to the color of the priest's vestments. I've heard that the Catholic Mega App or some similar app may have some of this functionality already, so this idea isn't completely original, but it'd still be cool.

### Catholic Bible.rs

[@DSpeckhals](https://github.com/DSpeckhals) has made an amazing [open-source PWA](https://github.com/DSpeckhals/bible.rs) for accessing the King James Version of the Bible. He's done a fantastic job, and it's obvious a lot of work has been put into making the app simple yet functional!

The only problem is that, as a Catholic, this Bible is [missing a few books](https://www.christianitytoday.com/history/2008/august/why-are-protestant-and-catholic-bibles-different.html). It'd be nice if there was a Catholic translation of the Bible here which included these missing books. The [Douay-Rheims Version](https://www.gutenberg.org/ebooks/8300) is in the public domain, so it'd be nice if it were available either as a toggle on the main app or as a separate web app.

### Catholic Catechism CLI

The Catechism of the Catholic Church is an amazing resource which contains a summary of many of the teachings of the Catholic Church. It'd be amazing if this were to be accessible via the command line. On that thought, why not make the Summa and other great books accessible via the command line?

### Automatically format ProPresenter slides

When I'm at a church using ProPresenter, one thing always annoys me: inconsistencies. Why are there punctuation marks on this line, but not there? Why is this line capitalized, but not that one? Why aren't any two slides consistent in their formatting, either in the same song or between songs? Sometimes, it seems the sound techs are just out to annoy you! (And yes, I can say this - I was a sound tech, and I worked hard to make the slides consistent!)

What if there was a ProPresenter/OpenLP/etc. add-on that made the slides consistent? It wouldn't be perfect, but at least it'd help me and the few out there like me to be less distracted by the slides.

---

# Credits

All (future) images on the Github Pages site powered by IPFS

<img src="https://ipfs.io/ipfs/QmUnLW4zb4zQML87Lp9mp1Roz52TrqHkwk6yDV67tURnPy" alt="IPFS Logo" width="200">
