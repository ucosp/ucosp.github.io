---
id: 2363
title: 'Anton&#039;s Midway Update'
date: 2010-02-24T18:16:20+00:00
author: Anton Markov
layout: post
guid: http://ucosp.wordpress.com/?p=2363
permalink: /2009-2010/mercurial/2010/02/antons-midway-update/
categories:
  - Mercurial
  - Status
---
It&#8217;s hard to believe that we are already 1/2 way through the UCOSP Mercurial project. It has been an amazing learning experience from both a technical and a social point of view.

I started out this project with some limited experience of using Mercurial on my own system. Not only did I have to learn Mercurial in the context of a team, but I also had to put myself in the shoes of users very different from myself. We are working on features for large teams with large repositories who have different requirements from individual developers. I will get back to this later.

My experience with Python was equally limited. I had used it for a couple of school assignments in the past, but as most of you know, one-time throw-away assignment code is nothing like a mature open-source project. As the Python coding guidelines quote, &#8220;Code is meant to be read by humans and only occasionally by computers.&#8221; Python is a powerful language, and I&#8217;ve been blown away by how clear and concise the code is. On the other hand, like any powerful tool, it must be used wisely and consistently.

From a social point of view, this is my first experience contributing code to an open-source project. The basic concept of bug tracking, specifications, and code reviews were familiar to me from co-op terms, but they take on a new light in an open-source project. While there are three of us working on Mercurial from the University of Waterloo, and we have met to discuss our work face-to-face, we quickly learned that any important discussion must take place on the public mercurial-devel mailing list. It is tempting to talk and decide things amongst ourselves, but it is important to involve the other developers and users of Mercurial. This is especially important when modifying other people&#8217;s code or working with scenarios that we don&#8217;t have personal experience with.

We started off the semester poking around and learning about Mercurial. The real work started at the UCOSP code sprint in Toronto where we spent 3 days hacking away on Mercurial together, in the same room. We all had small warm-up projects to work on. I worked on an extension to cache the results of the &#8216;hg annotate&#8217; command which shows, for each line of a file, the last time when it was modified. This project went well and the code was polished up in another week. I&#8217;ve since released it publicly on Bitbucket, and it has been integrated into FogCreek&#8217;s Kiln product.

Our next challenge was the bfiles extension. The bfiles extension is designed to make working with large binary files more convenient. Instead of storing the entire history of every file in every clone of the repository, the history is stored on a central server and each revision is downloaded as needed.

We seemed to hit a slow period with bfiles. It is a large extension which messes with various internal Mercurial functions. Furthermore, our tasks were very broadly-defined. We spent three weeks discussing different approaches on the mercurial-devel mailing list and getting the functional specs right. Finally I was able to start coding over reading week, but I hit implementation decisions and went back to the mailing list to discuss them.

Greg Wilson has taken every opportunity to emphasize the importance of communication on this project. I couldn&#8217;t agree more. Writing this update has helped me to organize my thoughts. I am off to do work.

~Anton