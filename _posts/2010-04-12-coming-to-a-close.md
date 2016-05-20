---
id: 2725
title: 'Coming to a close&#8230;'
date: 2010-04-12T19:59:51+00:00
author: godfreychan
layout: post
guid: http://ucosp.wordpress.com/?p=2725
permalink: /2009-2010/flightsim/2010/04/coming-to-a-close/
categories:
  - FlightSim
---
Our [FlightSim](http://ucosp.wordpress.com/category/flightsim/) project has come to a close last week, after posting our [final delieverable](http://ucosp.wordpress.com/2010/03/31/final-deliverables-of-data-center-flight-simulator/). It&#8217;s been a long ride, so I thought I should take my time to write down my experience and what I&#8217;ve learned here.

Different from most of you, our project started at IBM&#8217;s lab, not at the St. George campus. On our first morning, all of us were invited to their lab at Markham. The lab itself is a really cool place, and the IBMers have treated us well. But to be honest, it&#8217;s not exactly the greatest experience. We were basically given a crash course on DB2, then the TE (which is the foundation that our project is building upon), plus some unsuccessful troubleshooting session on how to get both working on a Mac and Linux. Because the amount of information is SO overwhelming, by the end of the day, all I was left with is frustration and question marks. Heck, I don&#8217;t really understand the porject that well to begin with, but then it feels like I understand that even less when we leave the labs. As everyone have already started doing some coding in the UT campus, I thought we would be doomed.

On the second day, things start to look a bit better. Matthew gave us a walkthrough of the TE codebase. Overwhelming, still, but we are starting at least starting to see what this is all about. (The lack of projector is really leaving something to be desired&#8230; six kids staring at a ultra-high pixel density laptop monitor&#8230; not even funny!) We also did, in my opinion, one of the most important things for our project. We set up or communication channel (Skype) and a meeting time (Tues, Thurs). Yes, it&#8217;s taking a lot longer than it should, and it could be done more efficiently, but I believe it&#8217;s well worth the cost, we&#8217;ll talk about this more in a bit.

By the end of the code sprint, most of us still haven&#8217;t got of systems set up probably. But then I started to understand more about our project and it seemed quite a bit more approachable.

As we splitted and returned to our home city, the first challenge is to get things working on our end. This marks the first collebration of our team. Within days, the wiki is populated with detailed instructions on how to get things working and what works and what doesn&#8217;t. We also helped each other out on Skype. Perhaps it&#8217;s the frustration we have in common that really bonded the whole team together, and this helped to smooth things out a lot for the rest of the term. It still takes a few more weeks and a lot of help from IBM (esp Paul, you&#8217;re awesome!!) before our systems are truely functioning, but can at least start doing some useful work now.

My first assignment is to investigate the recurssive queries issue. Basically, I need to write a recurrsive query that saturates the CPU. It took me quite a while to figure out what that even means. This is pretty much my first official encounter with the massive DB2 system, so I spent a good amount of time researching and learning how to fight this little monster. After a lot of trial and error, I have sucessfully created a recursive query that does some interesting things. However, the result is quite disappointing. Although it took me days to write that query, it only took the database 5ms to execute it. Matthew suggested that DB2 might be doing some crazy optimization behind the scene for me. Although this attempt turned out fruitless, it was a good experience and allowed me to get myself familiar with the DB2 system.

I was then reassigned to work with Mike on his locklist overflow scenario. His scenario worked beautifully on his machine, so I took up the task to reproduce and record that on my laptop. However, after a night of trial and error, I still cannot reproduce the problem on my own machine. I did some extra research and concluded that the behavior might under this situation is undefined, so it varies wildly across machines. I looked into the nature of the problem and proposed some changes to the scenario (changed from locklist overflow to lock escalation). Although we didn&#8217;t end up using this scenario, we did some serious work reseearching that problem, and left some pretty good foundation for other people to pick that up in the future.

To avoid slowing down our progress due to the extra work needed for the lock escalation scenario, I picked up on Sylvian&#8217;s lock wait scenario because it&#8217;s much simplier to reproduce and understand. We then continued our work based on this senario and ultimately produced a working version of our scenario and attached it in the final delieverable.

* * *

## What I have learned&#8230;

### 1. Reading other people&#8217;s code

By far, I think this is the most valuable experience for me. In the real world, developer documentation is a luxary for lot of open source projects. Having the experience of reading and understanding other people&#8217;s code will allow me to contribute to a wide range of open source project in the future.

### 2. Working within a distributed team

This is probably one of the most important that Greg planned this course for us. I realized how important it is to maintain good communication with the team. What makes our team unique in UCOSP is that we have two weekly meetings, one via conference call, one via Skype chat. Although this could be overwhelming at first, I do find this highly valuable and would recommend other teams in UCOSP to do the same.

### 3. Asking help

Without the help from IBMers like Matthew and Paul, we wouldn&#8217;t have gone this far for this project. I learned to ask help when you need it, and more importantly HOW to ask help. Describing a complicated problem clearly (but overwhelming) could be challenging and this course turned out to be an excellent opportuinty for practicing that.

* * *

## What I liked&#8230;

  * The semi-weekly meetings!
  * IBMers are very helpful&#8230; and often respond within ours of us asking a question.
  * The project was challenging, in a good way.

* * *

## What could be better&#8230;

  * The initial project definition was too vague&#8230; Because most students joining this team will not have the experience needed for understanding the project, I think it&#8217;d be a better idea for provide more guidance and make things more concrete for them at the beginning. Then, allow them to have more flexibility as they learned more about the project. (i.e. provide some clear and rigid goals, instead of allowing us to make our own goals right from the start, because we wouldn&#8217;t be able to take advantage of that flexibility at that time anyways)
  * The pieces we are building upon wasn&#8217;t quite ready for prime time yet when we first started, which caused a lot of frustration as we spent most of our time debugging and setting things up in the first few weeks. I believe this has mostly been addressed by now, thanks to the new releases and the sandbox server.
  * More documentation would be nice 🙂
  * The code sprint was quite overwhelming for most of us.. maybe we can aim to do/learn a little less at the sprint..?

* * *

Again, I would like to thank the IBMers (esp Matthew and Paul) for providing us such an incredible experience!