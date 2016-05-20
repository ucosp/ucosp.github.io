---
id: 1261
title: 'Status Report: Nov 11, 2009'
date: 2009-11-11T19:12:14+00:00
author: Dwight Deugo
layout: post
guid: http://ucosp.wordpress.com/?p=1261
permalink: /2009-2010/uncategorized/2009/11/status-report-nov-11-2009/
categories:
  - Uncategorized
---
## **Peter**

### Status

  * 6 tutorials worked on with Maciej completed and submitted, bug 290673.

### Next Steps

  * Working on Project Explorer, bug 294015.

### Roadblocks

<ul type="disc">
  <li>
    Operating System Class
  </li>
</ul>

* * *

## **Dennis**

### Status

  * Compiled survey results and published to blog.
  * Created a patch for Bug 293888, Adding line-numbers to the Scheme editor by default. 

### Next Steps

  * Working on Bug 293850, Adding a REPL View to the Scheme Presective.

### Roadblocks

<ul type="disc">
  <li>
    None
  </li>
</ul>

* * *

## **Nil**

### Status

  * Added 2 bugs and participated in the discussion: Bug 293838 : Scheme Help View and Bug 294487 : Scheme Play button.
  * Provided view on the scheme Package explorer that Peter is working on, bug 294015.
  * Helping Peter understand Help view.

### Next Steps

  * Continue with bugs 293838 and 294487
  * Making a Scheme Parser with Maxime using the JParseC library (Apache license). 
  * It&#8217;s not yet finished, but I&#8217;m sure it&#8217;ll be done next week. 

### Roadblocks

<ul type="disc">
  <li>
    We put a stop to the parser because Dennis wanted us to submit the SchemeWay perspective.
  </li>
  <li>
    Parser is already in our SVN, but we still need to clean some parts.
  </li>
</ul>

* * *

## **Maxime**

### Status

  * Wrote to Per Bothner about the files having licensing issues in Kawa and he was very helpful and we managed to fix them pretty fast.
  * Nil and I worked Bug 293093 (Scheme Perspective) making a cleanup of the dependencies and enforcing a uniforme code style.
  * Nil and I also made a Scheme parser, which is more than an S-expression parser. We need to have an "abstract syntax tree" of the code and not all semantic annotation. This way we will be able to know the variables available in each scope for the code-completion and to improve the code navigation "like word navigation but for the s-expression". We used a Parser combinator library http://jparsec.codehaus.org/.

### Next Steps

  * I am now really confident about the Kawa interpreter and we will build over it.
  * We will have to drop the "breakpoint" support, Bugs 242444 (Scheme Plug-ins initial contribution)

### Roadblocks

<ul type="disc">
  <li>
    None
  </li>
</ul>

* * *

## **Maciej**

### Status

  * Dennis and I agreed that we only need one person working on the REPL and so I selected another bug.
  * I will now be working on the HTML view for displaying help (Bug 293838). Peter was originally supposed to work on it but decided to do the Project Explorer instead.
  * Spent most of the time this week reading the code that I&#8217;m stating to build with. 

### Next Steps

  * Will continue working on Bug 293838 (Scheme Help View)

### Roadblocks

<ul type="disc">
  <li>
    None
  </li>
</ul>

* * *