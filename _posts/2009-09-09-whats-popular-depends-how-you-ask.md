---
id: 596
title: 'What&#039;s Popular Depends How You Ask'
date: 2009-09-09T19:22:18+00:00
author: Greg Wilson
layout: post
guid: http://ucosp.wordpress.com/?p=596
permalink: /2009-2010/education/2009/09/whats-popular-depends-how-you-ask/
categories:
  - Education
---
An ex-student of mine is trying to decide what web technology to use in the project he&#8217;s about to start working on.  The three choices are Java plus some kind of framework, Django and Python (which he knows very well), or Ruby on Rails (which he doesn&#8217;t, but could pick up quickly).  The argument in favor of Java plus whatever is that his employer is sure to be able to hire good Java programmers at a reasonable price for the next decade, but as he points out, doing small or medium-sized project in Java takes longer and hurts more than doing it in a dynamic language like Python or Ruby.

But what about Django vs. Rails? Is one more widely used than the other?  That&#8217;s usually a pretty good guide to how easy it will be to hire programmers who already know it [1], and how quickly libraries or adapters for [name of next year&#8217;s hot new technology goes here] appear for it.

In the past, I&#8217;ve relied on book sales, or even just the number of books on a topic, to tell me how much programmers care about something. My ex-student tried something else: a [Google Trends query](http://www.google.com/trends?q=django%2C+ruby+rails&ctab=0&geo=all&date=all&sort=0) comparing &#8220;django&#8221; with &#8220;ruby rails&#8221;:

<img class="alignnone size-full wp-image-597" title="first" src="http://ucosp.files.wordpress.com/2009/09/first.png" alt="first" width="580" height="260" srcset="http://ucosp.ca/wp-content/uploads/2009/09/first.png 580w, http://ucosp.ca/wp-content/uploads/2009/09/first-300x134.png 300w" sizes="(max-width: 580px) 100vw, 580px" />

I was very surprised: my impression had been that Ruby on Rails was much more widely used than Django. But then I looked at the query itself a little more closely, and decided to try two others. The [first](http://www.google.com/trends?q=rails%2C+django&ctab=0&geo=all&date=all&sort=0) compares &#8220;rails&#8221; to &#8220;django&#8221;:

<img class="alignnone size-full wp-image-598" title="second" src="http://ucosp.files.wordpress.com/2009/09/second.png" alt="second" width="580" height="260" srcset="http://ucosp.ca/wp-content/uploads/2009/09/second.png 580w, http://ucosp.ca/wp-content/uploads/2009/09/second-300x134.png 300w" sizes="(max-width: 580px) 100vw, 580px" />

That&#8217;s a very different answer, but looking at the results, it&#8217;s also untrustworthy, since &#8220;rails&#8221; includes web traffic about trains. How about [trying](http://www.google.com/trends?q=ruby+rails%2C+python+django&ctab=0&geo=all&date=all&sort=0) &#8220;ruby rails&#8221; vs. &#8220;python django&#8221;:

<img class="alignnone size-full wp-image-599" title="third" src="http://ucosp.files.wordpress.com/2009/09/third.png" alt="third" width="580" height="260" srcset="http://ucosp.ca/wp-content/uploads/2009/09/third.png 580w, http://ucosp.ca/wp-content/uploads/2009/09/third-300x134.png 300w" sizes="(max-width: 580px) 100vw, 580px" />

Which is the &#8220;right&#8221; answer? I have no idea. The last one corresponds most closely with my preconceptions, but I&#8217;ve been bitten enough times to recognize [confirmation bias](http://en.wikipedia.org/wiki/Confirmation_bias) when I commit it :-). [Rails Pub Night](http://unspace.ca/innovation/pubnite) in Toronto draws ten to twenty times as many people as meetings of the [Toronto Python Users&#8217; Group](http://pygta.vrplumber.com/), but again, that&#8217;s not necessarily an indication of who&#8217;s using Django.

What else would _you_ try to figure it out?

[1] Yes, a good programmer can learn a new language in a couple of weeks, but mastering a web framework and the dozens of modules needed to build an industrial-grade app takes a lot longer&#8212;it&#8217;s like the difference between being able to ask where the bathroom is and being able to discuss literature.