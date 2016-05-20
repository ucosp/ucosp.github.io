---
id: 1484
title: 'Status Report: Nov 25, 2009'
date: 2009-11-26T14:52:30+00:00
author: Dwight Deugo
layout: post
guid: http://ucosp.wordpress.com/?p=1484
permalink: /2009-2010/eclipse4edu/2009/11/status-report-nov-25-2009/
categories:
  - Eclipse4Edu
---
## **Peter**

### Status

  * Good push to finished work on bug 294015. 
  * Decided to use the "empty project" wizard and the already created Kawa File wizard so that now they can be used to create a project and scheme files. 
  * Fixing NULL pointer exception when clicking a file in the explorer. I am pretty sure that it has to do with the fact that I used the Java Lite Explorer and it is looking for the java lite editor which doesn&#8217;t exist in Scheme. 
  * Dennis said that he would help me along with the explorer. I think that we should be able to get this done early next week.

### Next Steps

  * Work with Dennis to fix null pointer in explorer, that will finish bug 294015
  * Help Maciej with Help view bug 298383

### Roadblocks

<ul type="disc">
  <li>
    End of term crunch
  </li>
</ul>

* * *

## **Dennis**

### Status

  * Working on Bug 293838; will be completed by code freeze
  * Working on Bug 294015; will be completed by code freeze (Nov 29) 

### Next Steps

  * 

### Roadblocks

<ul type="disc">
  <li>
    End of term crunch
  </li>
</ul>

* * *

## **Nil**

### Status

  * I participated in the discussion on the following bugs: 294487,Scheme Play button, 295541 Scheme : parenthesis not matching
  * Meeting on IRC with the team.
  * Worked on the parser with Maxime.
  * Created JUnit tests for the parser. 
  * Investicating how to color in green the matching parenthesis (295541).
  * Removed the menu and two icons from Scheme4Edu (293093).

### Next Steps

  * By november 29, I want the non-matching parenthesis to be done. 
  * And, provide a set of tests for the parser. 

### Roadblocks

<ul type="disc">
  <li>
    End of term crunch
  </li>
</ul>

* * *

## **Maxime**

### Status

  * Helped Nil with issue we had with the REPL error message.
  * Fixed the issues we had with the scheme perspective: the code outline and the "Jump to Definition" was broken.
  * Changed the Scheme parser using the use the R6RS lexical syntax: 
      
    http://www.r6rs.org/final/html/r6rs/r6rs-Z-H-7.html#node\_sec\_4.2.1
      
    and R6RS Datum syntax :
      
    http://www.r6rs.org/final/html/r6rs/r6rs-Z-H-7.html#node\_sec\_4.3.1
  * This parser is finished and seem to work fine

### Next Steps

  * Need to add Semantic support to parser to know which variable is visible in each <body>
      
    Ex:
  
    (define <variable> <expression>)
  
    (define (<variable> <formals>) <body>)
  
    (lambda <formals> <body>)
  
    (let <bindings> <body>)
  
    (let* <bindings> <body>)
  
    (letrec <bindings> <body>)
  
    (letrec* <bindings> <body>) 

### Roadblocks

<ul type="disc">
  <li>
    End of term crunch
  </li>
</ul>

* * *

## **Maciej**

### Status

  * Still working on bug 293838 (Scheme help view), want to add scheme help to the IDE so that students can quickly look up functions, procedures, keywords, etc.
  * Located and ripped out the help pages from the LambdaBeans project (as suggested by Nil).
  * Added a dummy table of contents and an index to our plug-in.
  * Currently, we can press F1 to bring up the help view where our help pages will be visible.

### Next Steps

  * Add all the help pages to the table of contents and index all the pages.
  * After the indexing is done the user should be able to quickly search for the page they want. 

### Roadblocks

<ul type="disc">
  <li>
    End of term crunch
  </li>
</ul>

* * *