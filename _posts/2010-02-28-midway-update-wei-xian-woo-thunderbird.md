---
id: 2445
title: 'Midway Update &#8211; Wei Xian Woo (Thunderbird)'
date: 2010-02-28T14:53:14+00:00
author: wxwoo
layout: post
guid: http://ucosp.wordpress.com/?p=2445
permalink: /2009-2010/thunderbird/2010/02/midway-update-wei-xian-woo-thunderbird/
categories:
  - Thunderbird
---
I am not proud to say this, but my performance on Thunderbird could have been better.

**Am I behind?**

  * Yes, I am at least three weeks behind the schedule I set for myself. I would have liked to submit my first patch by the end of January, but I ended up doing that only in the third week of February.
  * At the start of the term, I broke down the feature I was responsible for implementing into reasonably sized pieces and estimated that each piece will take approximately 1-2 days to implement. Even at this point, I feel that those estimations were fair and achievable given what I knew about my schedule at the time.

**Why am I behind?**

  * The term turned out to be a lot busier than I originally anticipated &#8211; for school (assignments + a research assistantship) and preparation for external exams
  * Figuring out how certain pieces of Thunderbird code interact with each other and where certain things are took longer than expected. For example, where/when is the first Thunderbird main window created? (No, searching for &#8220;startup&#8221; and other related keywords did not help.)
  * I spent almost two full weeks understanding the various types of Mozilla unit tests and identifying one that can do what I need. Mozilla has 7-8 types of these, out of which only 3-4 of them are currently used in Thunderbird. This time I felt was badly spent because asking Blake (which I had to do anyways) would have gotten me an answer much quicker.

**What have I learnt up to this point?**

  * How Mozilla apps (in particular, Thunderbird) work. The whole idea of using JavaScript to implement a feature like session restoration and storage is pretty fascinating.
  * Writing tests &#8211; despite having five co-op work terms of development experience, I definitely learnt some good stuff about testing here.

**So, how&#8217;s the remainder of the term going to look like for me?**

  * Within the next 2-3 weeks, I hope to finish up the remaining pieces of the feature. In fact, my revised 1st patch is almost ready as I write this and should be ready for submission sometime today.
  * I hope to be able to work on at least one other bug for the final month, which will hopefully take less time to tackle now that I have better understanding of how things work in Thunderbird.