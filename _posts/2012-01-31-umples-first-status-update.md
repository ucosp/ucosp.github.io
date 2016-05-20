---
id: 2855
title: 'UMPLE&#8217;s first status update'
date: 2012-01-31T14:43:38+00:00
author: rtholmes
layout: post
guid: http://ucosp.ca/?p=2855
permalink: /winter-2012/2012/01/umples-first-status-update/
categories:
  - Winter 2012
---
James Zhao writes:

This is the first blog post from the UCOSP Umple Team for Winter 2012. We are working on [Umple](http://try.umple.org) project, which is a modeling tool and programming language which allows one to perform model-oriented programming.

My fellow USCOP colleagues have been working on some interesting projects. [Adam Dzialoszynski](https://code.google.com/p/umple/wiki/UCOSPLogAdamDzialoszynski) has been working on SQL statement generation, which allows Umple to generate an SQL database schema. [Sonya Adams](https://code.google.com/p/umple/wiki/UCOSPLogSonyaAdams) has been working on adding a new feature to the Umple language which allows a class to be declared as immutable. [Jordan Johns](https://code.google.com/p/umple/wiki/UCOSPLogJordanJohns) has been working on improving how code comments written in Umple code are saved and transferred to the compiled destination programming language code. [Luna Lu](https://code.google.com/p/umple/wiki/UCOSPLunaLu) is currently working on [issue 142](https://code.google.com/p/umple/issues/detail?id=142) which deals with a bug in the language where deletion on a object that has a 1-to-many association is not working. [Song Bae Choi](https://code.google.com/p/umple/wiki/UCOSPSongBaeChoi) is working on [issue 21](https://code.google.com/p/umple/issues/detail?id=21), where Umple in a certain circumstance generates uncompilable Java code.

[What I have been working on](https://code.google.com/p/umple/wiki/UCOSPLogJamesZhao) is to make the Umple compiler appear more like the gcc compiler. I have started by adding command line options to the Umple compiler, implementing some of the simpler command line options, such as printing the current compiler version number. I am currently working on a command line option feature, which can control the programming language Umple will output.

After having started working on Umple for three weeks, I have learned how to look at large projects with multiple components. Also now understand the use of ant build scripts, which will be very useful in the future. A challenge now is juggling time between my other busy courses and Umple work. I expect this to be a very important skill to have since I would like to participate in more OpenSouce projects in the future.

&nbsp;