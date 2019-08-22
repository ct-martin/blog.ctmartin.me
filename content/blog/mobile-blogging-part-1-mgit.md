---
title: "Mobile Blogging (Part 1): MGit"
date: Fri, 16 Aug 2019 22:13:00 +0000
draft: false
tags: ['Web Dev']
---

My boss's boss encouraged me to bring a Bluetooth keyboard on my flights this weekend so I could write while in the air.
Suprisingly it's possible to do this on Android directly using plain Git.

<!--more-->

For this to work there are a couple requirements:

* Content source must be in a git repo
  * If you're using WordPress there is a plugin to sync with a git repo but I haven't tested it so YMMV
* Something comfortable to type with, such as a (small) bluetooth keyboard
* An Android git client that:
  * Can clone the repo to local storage
  * Allows you to edit files
  * Allows you to commit & push files

Amazingly, there are not as many git apps that can do that as I thought there might be.
I'm an Android user and I chose to use [MGit](https://play.google.com/store/apps/details?id=com.manichord.mgit&hl=en_US).
There are other options available but few meet the 3 criteria for a git app I listed above and appear to be of decent quality.
There was at least one other quality git app I saw while searching, but it appeared to have some major issues with disconnect between the dev & users.

It's worth mentioning that you won't get prompted for HTTPS auth until you try to push on public repos since that confused me at first.

I did make an effort to try to find a good, free Markdown editor for mobile, however, I didn't find anything that matched my taste. Either they didn't have support for underscores for italics (which I prefer due to notable platforms that use sincle aserisk for bold), didn't format the Markdown in the same view as typing, or were going to be a notable hassle to move content back and forth from MGit.
Actually, there was one that seemed to meet all of those criteria but nominally the Markdown support is paid-only (even though it worked for me) and I ended up finding it easier to just write in MGit's editor.

Overall I'm fairly happy with the experience.
This is the second blog post I've written while on a plane and things seem to work overall; committing and pushing worked. I know I'll need to proof-read these posts when I have access to a internet & my laptop (for errors, getting links, adding screenshots/related images).
That said, I've written the words which is most (if not all) of the work.

And for [part 2](/2019/08/mobile-blogging-part-2-testing/), I also learned that I can preview articles for testing on my phone as well.