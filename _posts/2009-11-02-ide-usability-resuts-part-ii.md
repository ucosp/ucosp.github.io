---
id: 1182
title: 'IDE Usability Resuts &#8211; Part II'
date: 2009-11-02T03:44:41+00:00
author: dennisacosta
layout: post
guid: http://ucosp.wordpress.com/?p=1182
permalink: /2009-2010/eclipse4edu/2009/11/ide-usability-resuts-part-ii/
categories:
  - Eclipse4Edu
---
Maxime Caron recently posted [results](http://docs.google.com/present/view?id=addqfjnjc3d6_108gj3w67c3) from the [French version](http://spreadsheets.google.com/viewform?hl=en&formkey=dHRBS2l5S0M4anI2LWdEV3JEV0cxSmc6MA) of our survey. Here are some of the [findings](http://proton.scs.carleton.ca/~dacosta/ide4edu/results.ods) from the [English version](http://deugo.carleton.ca/ESurvey/participationPostSurvey.action?id=40288048247c506d01249110b7400002&password=) and how I interpret them. (Note: Unfortunately, the server that was hosting the survey had a slight meltdown (literally!). We were able to recover some data but not everything.)

The first five questions were used to gain an understanding of the user and their previous programming experience. This allowed us to interpret the results in the proper context. Of particular interest are the questions about IDE preference:

42% of participants have used Eclipse
  
23% of participants prefer Eclipse

The drop in user retention can be attributed to many different reasons, but the results may suggest that users are finding the standard Eclipse environment too complicated. These results are comparable to the French version of the survey.

Questions 6-10 were used to determine whether a feature is commonly used by a beginner programmer. The features in question are currently up for debate within the Eclipse community. Here&#8217;s what we learned:

73% of participants use a Debugger
  
88% of participants find a line-number &#8220;ruler&#8221; useful

The results suggest that users aren&#8217;t having a hard time using a debugger as originally assumed. This is significant for us because we were considering simplifying the Eclipse Debug Perspective but this may no longer be necessary or a priority. Also, line-numbers in the editor are currently not available by default in both the standard Eclipse environment and Eclipse4Edu. This is something we may want to consider including.

Questions 11-13 were aimed at determining whether specific features (compiling, execution, and importing/exporting) were complex for beginners. The results show that all of these tasks are easily accomplished or learned and therefore need little changing.

The final questions were open asking for any difficulties encountered, likes/dislikes, and feature requests. Here is a sample of the feedback:

&#8220;creating a project in eclipse is confusing because you need to actually right click on the src folder when you want to create a new java class. While this sounds extremely simple now, it was a task that I was almost ready to give up on when I tried to create my first project.&#8221; &#8211;**This is actually addressed in Eclipse4Edu.
  
** 

&#8220;For Eclipse, I wish it was easier to attach the java source code to the program. As it stands I have to install the jdk in order to attach the source. This isnt very handy when I&#8217;m on a network machine where I&#8217;m unable to install anything. Also I wish the program would tell me about such features as the debugger, revision control system and refactoring features because I have no idea what those are and would like to get the most out of the program. Finally I wish it was easier to search in Eclipse for java code. Having to use the hierarchy pane is complicated, I would like to just open a search window and type in what Im looking for.&#8221;****