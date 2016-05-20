---
id: 2382
title: 'Tim&#039;s Midway Update'
date: 2010-02-25T21:05:33+00:00
author: mille449
layout: post
guid: http://ucosp.wordpress.com/?p=2382
permalink: /2009-2010/uncategorized/2010/02/tims-midway-update/
categories:
  - Uncategorized
---
This semester has not been as productive as I would have liked.  I set out to fix a single [bug](https://bugzilla.mozilla.org/show_bug.cgi?id=494137) in Thunderbird that I thought would be cool to do.  Before I left code sprint I found I had to fix another [bug](https://bugzilla.mozilla.org/show_bug.cgi?id=515907) first to add support to fix the original.  Doing so would put my code in the base Mozilla library, which was used for Firefox also, so I thought this was exceptionally cool.  And all I had to do for the second bug was write a single interface function that was only a few lines long!! Easy, right?

Well, here we are at midway, and I finally submitted my patch for the second bug today.  It has not been reviewed or accepted, and I don&#8217;t have tests for it yet, which I need before it can be accepted.  It has been a long, agonizingly frustrating haul to get to this point.  One of  the biggest obstacles for me was the XPIDL interface that the Mozilla platform is based on.  I have had a decent amount of experience with C++, so I understood the errors I was getting, but I did not understand how my code was being used in the compile process.  I got it to compile at one point, but then did an update to my local repository and it would no longer compile.

This brings up the second big obstacle: the size of the codebase.  Searching though it was not really much of a problem because of the excellent cross reference site Mozilla has, but compiling was a nightmare.  A full compile takes at least 45 minutes on my computer.  I had to do this a lot more times than I should have because I did not know if there were problems with how intermediate files were being handled.

Also, the make files specified that the commands, as well as the output from compiling, should be output to the terminal.  These commands were often very long so reading compiler output when compiles failed was next to impossible.  Many times, I would have to look back through two to three screens of output to find the error that stopped the compile.  A number of times, I mistakenly tried to fix the second or third error, which came as a result of the first one. Fortunately, I recently found the silent option for make which made reading output immensely easier.

I have spent most of my time either waiting for compiles to fail or studying up on errors online.  I feel like one of those monks in Monty Python who keep banging their foreheads with a board.  Except that I&#8217;m using a keyboard.  Perhaps the most frustrating part of the semester, however, has been to talk to other people who are making a lot of significant contributions to the projects they are working on.  I feel like a useless programming noob because I can&#8217;t even get a few lines of code to compile and I don&#8217;t have anything to show for my efforts.

However, there is light at the end of the tunnel,  I finally got my code to compile today and submitted a patch. In the process of searching for solutions for my errors I found out I was doing other things wrong that would not have stopped a compile, but would have caused errors later and was able to fix them. I&#8217;ve learned a lot about the Mozilla platform and C++ and how you can use it.  Hopefully the second half of the semester will go better. I don&#8217;t think I&#8217;ll be messing with the same sort of code to fix the original bug, which could be good or it could be the same thing again.  Even if it does give me problems though, I feel like I have gotten better at finding solutions and should be able to handle them better.