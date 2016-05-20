---
id: 1156
title: Grading Scheme for RoboCup
date: 2009-10-31T02:17:52+00:00
author: kyokko
layout: post
guid: http://ucosp.wordpress.com/?p=1156
permalink: /2009-2010/robocup/2009/10/grading-scheme-for-robocup/
categories:
  - RoboCup
---
**Team Grade: 40%**

** _Performance of soccer team &#8211; 10%_**

  * Fails to beat original team &#8211; 0/10
  * Wins occasionally &#8211; 4/10
  * Consistently wins by narrow margin &#8211; 8/10
  * Consistently wins by large margin &#8211; 10/10

** _Report &#8211; 10%_**

Written report explaining everything that was accomplished, remaining problems, TODO for people who might be working with our code. Mark should reflect completeness, justifications and clarity of writing.

_**Documentation &#8211; 10%**_

Comments in code and design document.

_**Screencast Demo &#8211; 10%**_

Demo on YouTube or similar service showing a client running.

**_
  
_** 

**Individual Grades: 60%**

  * Participation &#8211; 10%
  * Testing &#8211; 10%
  * Completion of Tasks (Code Sprint, Individual Tasks) &#8211; 40%

**Participation &#8211; 10%**

  * Writing requirements: blog posts, minutes, etc.
  * Meeting attendance, communication skills, etc.
  * Peer evaluations

Each team member had some tasks assigned. For this project it was hard to find completely non-overlapping problems for each member to work on, also tasks got reassigned occasionally for various reasons. Our individual grading schemes are taking that into account.

<span style="font-family:Helvetica, 'Times New Roman', 'Bitstream Charter', Times, serif;"><span style="font-family:Georgia, 'Times New Roman', 'Bitstream Charter', Times, serif;"><strong><em>Testing/Performance &#8211; 10%</em></strong></span></span>

<span style="font-family:Helvetica, 'Times New Roman', 'Bitstream Charter', Times, serif;"><span style="font-family:Georgia, 'Times New Roman', 'Bitstream Charter', Times, serif;">Note: RoboCup is a real-time running application, so for most of the functions it is impossible to create Unit tests. We use Debug UI and Human Controlled player to evaluate performance of the client. </span></span>

<span style="font-family:Helvetica, 'Times New Roman', 'Bitstream Charter', Times, serif;"><span style="font-family:Georgia, 'Times New Roman', 'Bitstream Charter', Times, serif;">Testing for people working on incorporating Machine Learning (ML) algorithms for high-level decision-making is a standard procedure which involves creating a test dataset and using it to assess how well the trained model generalizes to new data.</span></span>

**_Tasks from code sprint weekend &#8211; 10%_**

  * Ioana/Chani &#8211; Debug UI
  * Patrik/Yulia &#8211; Human Controlled Player ver.1
  * Alex &#8211; Java Monitor

**_**Individual tasks &#8211; 30%**_**

These are projects each person has been working on since Code Sprint. Since we all focused on different tasks, individual grading schemes reflect the amount of effort put into particular area.

_Chani_

  * Basic Actions (-improvements to basic actions: kicking, dashing, turning, etc) &#8211; 15%
  * Complex Actions (developing multi-tick actions, that are based on the basic actions and allow for more complex behaviour : dashing to position, following the ball, finding the ball when it hasn&#8217;t been seen for a while, etc) &#8211; 15%

_Ioana_

  * Sight Improvements (integration of better vision algorithm into the complex actions)  &#8211; 15%
  * ML (using Decision Trees (DT) or Neural Networks (NN) for better decision-making)- 15%

_Alex_

  * ML (experiments with various parameters for DTs and bugfixes to parser) &#8211; 15%
  * Actions (debugging and improving basic actions and multi-tick actions, in particular better passing) &#8211; 15%

_Yulia_

  * ML testing and experiments  (creating dataset for evaluation of ML algorithm&#8217;s performance, various experiments with different training data and parameters) &#8211; 15%
  * ML infrastructure  (parser for server logs, Human Client ver. 2, script to feed data to ML algorithm) &#8211; 15%

_Patrik_

  * Basic actions  (debugging and improving algorithms for basic actions : kicking, turning, seeing, etc) &#8211; 15%
  * Complex actions  (multi-tick actions, that are composed of basic actions and enable more complex behaviour: interception, dribbling to a position, chasing the ball, etc) &#8211; 15%