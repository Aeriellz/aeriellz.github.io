---
categories: compsci
date: 2026-09-23 12:36:00 -0300
title: expansion
layout: post
tags:
  - code-learning
  - homelab
lang: eng
ref: expansion
---
Having finished the NAS setup and learned a lot about it, over the last few months, I then took a long awaited pause to just bask in the fact that I now had a good and safe place to store files, and back up my writing, photographs, and things I didn't want to leave in someone else's computer. And in the meantime a lot happened. AI bullshit kept bullshiting, the price of storage memory and literally everything else started making everyone want to commit crimes, a friend started his own server, and I remembered I had three old computers lying around that another friend decided was junk and that I was the best one to unload it on.

Jokes on him.

While he did take the hard drives out for his own storage, he left me with the boards and the processors, which are not at all new, but usable. I'm running the current NAS out of an old RPi 3 B, but what if I could upgrade myself into something that has a little more power? It's all 4th Gen Intel processors, some more useful than others. But. It's literally free real state—or, as it became the norm to say, *compute*. Those are all laptop boards, too, so low power.

The idea came so easy it should've scared me; it was really the natural next stage: *what if I cluster them?*

And thus I go into the next layer of the homelab, and a few more headaches come with it. The plastic on those old laptops was so old and awful there wasn't much else to do but disassemble it all and get the bare boards. That is, incidentally, what they have IT people do when they inevitably end up in hell. Disassemble old laptops to the bare boards for the whole of eternity.

My partner, a software engineer, saw the mess on the living room and made a face.

"Ew. *Hardware*."

I say we make a great team. I'm not exactly fond of coding when I can just happily snort the solder fumes. You know that's a better death than trying to get C code to function. Why am I coding in C? 

Shut up. That's why.

And I'll gratefully leave her to deal with it or whatever else she thinks is better. What happens between her and her indentations is none of my business.

Anyway, it's a little bit of a journey, now, to understand exactly what I need for my intended set up. It's starting with finally going into understanding Docker permissions, which is leading me into a bit of a rabbit hole of network security. From there I will most likely need a network switch—that makes me giddy because it look so *hackery* to have one of those around—, and then I'll need to figure out what the fuck I'm gonna whip up to house the boards and the switch and I'll need to find a way to power these, and I'll need some thumb drives to run the OSs, then I'll need to actually cluster them, which, god knows how *that* works, and then I'll need to—

Headache. Migraine, even.

One bite at a time.

Before all of that there's some file juggling because all my shit is scattered in drives and I need to better use my resources on that front. I'm learning that a lot of administering servers and networks is being smart around allocation and permissions. Not worth it using a 1Tb drive to house 1Gb of OS. Specially when you don't really want that same drive being used by Docker. And that means planning.

It's back to the drawing board for me, for now.