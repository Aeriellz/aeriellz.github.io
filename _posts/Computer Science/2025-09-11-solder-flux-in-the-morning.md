---
categories: compsci
date: 2025-09-11 18:37:00 -0300
title: i love the sweet smell of solder flux in the morning
layout: post
tags:
  - code-learning
  - homelab
---
Ever since I started going into coding I knew that eventually I wanted to run my own server. It started as me wanting to serve this website myself, mostly for fun, because I'm pretty sure that might be unsafe if not done right (I have not yet researched into, specifically, serving websites), but it quickly became something else. To make me even more convinced that relying on cloud storage is not for me, I just had all my files deleted from Mega because my account wasn't active enough. They send emails and wait, but the account and that email were 10 years old, I didn't see it on time. Everything I had from my teen years is now lost to entropy, and that has a way to make a girl mad. Those weren't files that I had any realistic use for, but it put it in perspective that bytes are fragile, and that "*the cloud*" isn't archival.

So server it is. It's something that the 12 year-old me that still lives in my heart thinks it's really *1337*, and *cool* 😎, and because now I am an adult I have absolutely no reason to *not* do it. Other than the price of storage drives.

Now, my solution for this starts back when I was still in college and a friend, who worked at the repair shop we had there for cameras, was kind enough to part with a RaspberryPi 3 Model B he had lying around and had no use for. This guy is the reason I know how to solder cables and that I can change blown capacitors. He taught me how to not electrocute myself, and was always encouraging of my curiosity towards electronics. He was also profoundly ADHD, possibly insane, and failed to deliver in his the promise of using duct ape to glue me the ceiling of the Externals lab.

Now, because all the electronics he had and worked with were part of a filmmakers effort, and other video research, his raspberryPi was a little... different.

![A RaspberryPi 3 Model B, in a gutted D-link case, with a lot of wires soldered to it](/assets/RaspPi-before.jpeg)

Some of it is understandable: he needed a coaxial connector for video in addition to the HDMI, for example, so he just tacked one in there. But why, God, *why*, would someone mount it upside down inside a fucking D-Link router case and cover the original USB plug, just to solder in a harder-to-find, more cumbersome, power plug?

A track to a another friend's house later and I had it attached to a TV to use as a monitor (since I don't have one), reinstalling Raspibian, just to start from scratch. Then came the fumbling with old broken keyboards, cheap mouses, and a longer-than-recommended daisy chains of adapters, because when you start messing around with electronics and hobby tech no one tells you that you won't have what you need at first.

Not ideal, but it worked. Software-wise, everything was fine.

![A RaspberryPi 3 Model B, in a gutted D-link case, with a lot of wires soldered to it](/assets/raspPi-InitialsetUp.jpeg)

Thing truly started getting into a different territory when i realized that, because of the way everything was soldered together, I would have to get it *out* of the router case. It was not strictly necessary for me to undo all this work, since this little buddy will just stay in a corner of the room attached to as many drives as I can get away with, but not only the aesthetics of it bothered me—I am, first and foremost, an artist—, the HDMI extender the original owner bodged together wasn't reliable enough and was constantly making me lose image. Eventually I'll just SSH it, but for the time being I *need* to see.

Out of the gate a couple of screws broke inside the pillar extenders, because... god knows why, I don't fucking know. Some of the solder was thicker than I knew what to do with, too, and I don't have a solder wick. All of it was just made to *not* be undone and here I was defying the most basic of all principles: if it ain't broke, don't fix it. The punishment for this crime was a few fingers burned, almost setting fire to a table, and a mini-heart attack: I ripped a pad in the kerfuffle to undo a particularly finicky solder.

It was the last jumper I had to detach and after I did the Pi would just red light on me without turning on. Those are still pretty expensive here, and I wasn't excited to buy a new one. Then it turned out I was just dumb, and had forgotten I'd taken out the miniSD from the bay to work the solders. The PP6 pad I ripped was apparently to ground, and not necessary to the overall function of the system.

It was fun work, and learning this kinda stuff is truly just being a blast. I love hardware work, even more than software, because something about just getting some rocks to come to life and think feels like magic.

Next comes some research, and spending money. I can't use my friend's TV forever, and I'll have to check how to actually make this into a server. It's a bit scary, but I'm hella excited. At least from now on if I lose files I have only myself to blame.