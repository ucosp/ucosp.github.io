---
id: 2646
title: Pony-Build Spring Break Update
date: 2010-03-13T19:56:07+00:00
author: kshakyaz
layout: post
guid: http://ucosp.wordpress.com/?p=2646
permalink: /2009-2010/uncategorized/2010/03/pony-build-spring-break-update/
categories:
  - Uncategorized
---
This Monday instead of our regular conference call over Skype, we decided to not to have a conference call. We did not have much to talk about. So we decided to take a break and just send our weekly updates in the mailing list. Here is the part of the email.

Jack:

“_I&#8217;ve still been working on the parser for new build scripts, want to do a bit of cleanup on it tomorrow and then try integrating it into the pony-client script itself in the next few days.  What I&#8217;ve been working on so far is all checked in under my pony-client_rework branch:</p> 

</em> <a href="http://github.com/JackCarlson/pony-build/tree/pony-client_rework" target="_blank"><em>http://github.com/JackCarlson/pony-build/tree/pony-client_rework</em></a>_</p> 

My work is mostly in the added file &#8220;clients/testConfigAndBuildParser.py&#8221;&#8211;those functions form the core of what I&#8217;m currently planning on integrating into pony-client.py.  I have two other files added&#8211;pony-client.config, which stores default information (such as build servers, etc), and quixote.pb, my test Quixote build script.  quixote.pb is ugly for a reason at the moment, was testing various error conditions, but the gist of it is all there.”</em>

Max:

_“What I have been working on&#8230;..</p> 

Been messing around with the timeout stuff, have to test the code now.
  
See my subprocess branch for the changes I made to \_run\_command.

&#8220;What I want to work on&#8230;..&#8221;

This week I am going to go back and work on pip failure again, now that you have gone through and refactored a lot of things.
  
I am all so eying one of the other issues to work on, or maybe I will look over IDEAS/projectlets and see if anything catches my fancy. Will update list next day or so with what I decide.”</em>

Fatima:

_“For the build-mock I have made the changes made on mock.py to fix the magicMethod that was failing for me , but was still getting the same error. I then contacted Micheal Foord who explained that test wasn&#8217;t fixed and that he will try to include it in the next release of Mock 0.7.0.
  
On the other hand , I have created a bickbucket account and forked your Pony-build-test-hg repo to start experimenting with branches.
  
Using non-default branches is not typical as Augie explained earlier , but wanted to experiment with the named branches.”_

Khushboo:

_“I have not much to report because I have not been able to do much since I was/am out of state. But I will be online in skype though. This week I have been working on getting my mechanize package to run. But I trying to fetch Titus&#8217;s repo but I am getting the denied permission.Also regarding the nose package, I need fetch some branches which I am trying to fix. Thats it so far.”_