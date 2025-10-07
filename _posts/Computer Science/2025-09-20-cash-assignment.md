---
categories: compsci
date: 2025-09-20 10:41:00 -0300
title: "cs50, part i: the cash assignment"
layout: post
tags:
  - code-learning
  - cs50
lang: eng
ref: cashassignment
---
This was truly a fucking time.

I've had a hard time with the anything regarding logic and math as a kid, and as silly as it sounds it bounced of a lot of insecurities and other stuff that made me miserable for the rest of my life. It's a long story, but suffice to say, coding kinda triggers some of that and it makes everything harder than it has to be. I saw the cash assignment and completely froze, at first, because I was trying to do it mathematically, instead of logically, which was a complete waste of time.

I've been writing the code and making notes of my experience and thought process as comments, so I can track my progress and my mistakes. A friend of mine who's a developer complained about the excessive commenting, because apparently "you're not supposed to do that", but tough luck buddy. It's not for you. It's helping me learn, and that's all that matters.

```c
// ---- COMMENTS ON MY EXPERIENCE WRITING THIS ----
// Here's the thing with this code, and where you were having a hard time:
// you kept thinking about a math way of doing it,
// like, you went as far as "oh maybe modules",
// jesus, girl, bring it back to the basic!
// really, you can do all of this proceduraly,
// which is how it's easier to figure this out.
// let the computer do the math for you
// divisions and multiplications are nothing but loops and recursion
// of addition and subtraction
// don't try to make it smart. just try to make it.
// let the computer be math smart for you.

// also, remember what's behind do/while/for loops,
// when it's better to use each one of them.

// everything else is the boring ass things from C syntax
// which can be a pain, but just a matter of correcting it
```

Now, that last part was *fun*. The code wouldn't even compile and it took me a whole 10min to understand how the syntax of function definition works, and it only took me just that because I had help. I might hate AI, but the duck debugger is a game changer for learning code. My conversations with it would be funny if they weren't despair inducing. My conversations with my partner are even better.

![](https://i.ibb.co/WWPDqTCp/Screenshot-2025-05-27-at-17-30-42.png)

![](https://i.ibb.co/yB7ZR7Z7/Screenshot-2025-05-27-at-17-23-25.png)

The problem was that a function doesn't need a parameter if it's going to work with global variables. Sounds obvious, but no one tells you that, like no one tells you that the global variables are going to be updated by whatever function uses it, and parameters will just use a copy of the original value. This simple paragraph is fast to write, but when code goes wrong it's not fast to understand why, no matter how dumb the problem is, and it's usually dumb.

I made a copy of the file so I could do both and see which one I liked better. Once I decided for global variables and finally managed to get it to compile, I knew it wasn't gonna run smoothly and probably be every single kinds of wrong, but I had no idea the level of problem that first problem with the global variable would land me in.

In coding, as in life, errors cascade. I've learned that the worst ways.

It took me *hours* to figure out that, when I took the parameters out, things still needed to actually match and look like one another. Half the code was written for global variables and the other half was written for parameters. I had to fix some stuff. Once the realization set in, it wasn't much of a problem. I just moved the math to a different place, and it should work!

Except it didn't. And I couldn't for the life of me understand why. It was compiling fine, the math was sound, the code should work. Why the *fuck* wasn't it working?

At that point the code should be so simple that the duck could help us debug, and our own minds could do the rest, so no one explained to us how to use VSCode's debugger. I spent 3 days trying to understand what was happening. I took the comments out. I rewrote the whole thing. I went line by line with the duck, asking if my logic was right. Then I went line by line in my own head, following the code like the computer would. Each time the result was the same: it should be working.

Yet, time and time again, I would press *up*, and then *enter*, to run the file through the command line, and the code would still be broken as if I never fixed anything. I was going completely insane. Hours of duck. Hours of thinking I was even worse at math than I thought I was if a simple addition operation wasn't working. 

My last ditch attempt was something I remembered Daniel Shiffman, from [Coding Train](https://thecodingtrain.com), doing when he's got bugs. He prints all the values from his functions to the console at important steps, and tries to figure out where the hell the computer is getting those values from. So printf I wrote. It compiled. I ran it... and... it wan't printing anything?

Panic set in for a total of half a second before I pressed *up* to bring up the last command I ran on the CL. It was the wrong file.

For three days, I was running the wrong file.

![](https://i.ibb.co/NRVKDsL/Screenshot-2025-06-20-at-18-03-16.png)

The only reason I didn't start crying was because I was not home. Me and a friend went to study at a coffee shop. Once I ran the right file everything was working perfectly. It was a victory, and while I was not pleased with it, I managed to laugh it off.

All of this was about a month ago, and then for my own sanity I took some time before starting the next class. I watched it, but I haven't started the problem set yet. We all have *that* disaster to look forward to. 

### Key takeaways

1. **Global Variables**: When you use global variables, any changes made to them within a function will affect the original variable.

2. **Function Parameters**: When you pass a variable as a parameter to a function, the function works with a copy of that variable, so the original variable is not modified.

3. **Debugging**: printf is a miracle and should be used whenever possible.

4. **Check your files**: don't be me.

5. **You will make mistakes:** dumb ones. It's fine. It doesn't say anything about you other than that you're doing well.

