---
title: Mobile Blogging (part 2) testing wih Hugo
date: Mon, 19 Aug 2019 15:52:00 +0000
draft: false
tags: ['Web Dev']
---

**PROOF CHECK: IS `pkg-config` NEEDED?**

Today I learned that I can run Hugo to preview my blog posts on my phone in addition to [writing them](???).

<!--more-->

As it would turn out, someone made an app to run Linux on Android.
I'm amazingly not suprised about that somehow.
The app is called [Termux](???).

Anyway, to get my blog to an accessible location I had to change MGit's base directory in the settings, which also made me re-clone my repo.
Thankfully I hadn't written anything at that point because I don't know what the default location is.
I also recommend using the Downloads folder for this as Documents isn't accessible in Termux.

In Termux there are two package managers, `pkg` and `apt`.
As far as I can tell, `pkg` is a wrapper for `apt` with a couple minor changes such as a different help output.

Use `apt install proot` to get Proot, which is a user-space chroot implementation we need so things think they're running on Linux (Termux doesn't comply with the Linux/Unix filesystem standard).
Then use `termux-chroot` to enter into the chroot.
You probably won't notice anything different about running in or out of the chroot for the most part, or at least I haven't.

After that you can use `apt install hugo`, which is also conveniently the "extended" version of Hugo so you get SASS support.

Add a `cd storage/downloads/Git/blog.ctmartin.me` and a `hugo serve` and you're all set!

Despite running a server, this is airplane-mode compatible since it's all local to the phone.

Easy go!