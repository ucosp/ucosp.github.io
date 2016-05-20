---
id: 2187
title: Technology Explorer Introduction
date: 2010-01-28T19:52:49+00:00
author: Diane Tam
layout: post
guid: http://ucosp.wordpress.com/?p=2187
permalink: /2009-2010/flightsim/2010/01/technology-explorer-introduction/
categories:
  - FlightSim
tags:
  - FlightSim
---
<span style="text-decoration:underline;"><strong>Technology Explorer for IBM DB2 &#8220;Flight simulator&#8221; Project</strong></span>

**Team:**<span style="text-decoration:underline;"><strong><br /> </strong></span>

_Brian Olynyk, team lead of Technology Explorer_

_Peter Kohlmann, original creator of Technology Explorer_

_Matthew Vandenbussche,_ _core developer and_ _architect of_ _Technology Explorer_

_**<a href="http://ucosp.wordpress.com/winter-2010/" target="_blank">UCOSP Students</a>:**_

[Michael Man](http://ucosp.wordpress.com/2010/01/05/michael-man/) SFU <[mantong01@gmail.com](mailto:godfreykfc@gmail.com)<a name="12638d4e63e1a2c9__MailEndCompose">></a>

[Godfrey Chan](http://ucosp.wordpress.com/2010/01/05/godfrey-chan/) SFU <<godfreykfc@gmail.com>>

[Lenny Han](http://ucosp.wordpress.com/2009/12/19/lenny-han/) Toronto <<a href="mailto:fallingangeles@gmail.com" target="_blank">fallingangeles@gmail.com</a>>

[Diane Tam](http://ucosp.wordpress.com/2009/09/09/diane-tam/) Toronto <<a href="mailto:diane.tam@gmail.com" target="_blank">diane.tam@gmail.com</a>>

[Jean Lalande](http://ucosp.wordpress.com/2010/01/14/jean-lalande/) Laval <<jeanlalande@gmail.com>>

[Sylvain Petitclerc](http://ucosp.wordpress.com/2010/01/13/sylvain-petitclerc/) Laval <<sylvain.petitclerc@gmail.com>>

**_UCOSP FlightSim Team Blog:_**

<a href="http://ucosp.wordpress.com/category/flightsim/" target="_blank">http://ucosp.wordpress.com/category/flightsim/</a>

_**Weekly Team Meetings:**_ 

Tues and/or Thurs 1-2pm (EST)

_**Code Sprint Jan 15-17 Overview:**_

<a href="http://ucosp.wordpress.com/2010/01/17/day-3-database-flight-simulator/" target="_blank">http://ucosp.wordpress.com/2010/01/17/code-sprint-day-1-2-data-server-flight-simulator4/</a>

<a href="http://ucosp.wordpress.com/2010/01/17/day-3-database-flight-simulator/" target="_blank">http://ucosp.wordpress.com/2010/01/17/day-3-database-flight-simulator/</a>

**Overview:**

_One of the major long term goals for the Technology Explorer for IBM DB2 has been to provide an environment similar to a flight simulator for Database Administrators.  Pilots used to learn to deal with potentially dangerous and stressful situations in a real place.  This was risky and expensive.  Pilots today learn to deal with system failures and extreme conditions on flight simulators.  DBAs still develop their experience on live multi-million dollar production systems.  They could develop skills and confidence faster and more safely on a simulator._

_Over the past few years the Technology Explorer for IBM DB2 team has built all the base components to create this simulator as part of our open source project.  The next step is to pull the pieces together into a viable simulation.  The team will use the existing open source building blocks to simulate a stable production system and then disrupt it with a number of planned or unplanned problems.  The system will then walk the DBA through problem recognition and resolution._ 

_Goals for the project would:_

  * _Extend the existing framework to simulate database management problems_ 
      * _Simulate DB2 in production_
      * _Create a disruption of the system, for example a hard drive failure, lock contention, or excessive workload_
      * _Guide a DBA to identification and resolution of the disruption_
  * _Develop at least one example of a problem simulation_

**Languages:**

_PHP, JavaScript, Prototype js library, AJAX, dynamic web pages, HTTP protocol (the impact of it being a stateless system and what has been done to keep memory between requests on both the client and server sides)_

**Project managed through <a title="SourceForge.net" href="https://sourceforge.net/" target="_blank">SourceForge.net</a>:**

Wiki: <a href="http://db2mc.sf.net/" target="_blank">http://db2mc.sf.net</a>

Development:  <a href="https://sourceforge.net/projects/db2mc/develop" target="_blank">https://sourceforge.net/projects/db2mc/develop</a>

Forum: <a href="https://sourceforge.net/projects/db2mc/forums/forum/761211" target="_blank">https://sourceforge.net/projects/db2mc/forums/forum/761211</a>

Issue Tracker: <a href="https://sourceforge.net/tracker/?group_id=211760" target="_blank">https://sourceforge.net/tracker/?group_id=211760</a>

**Additonal Links:**

Steps for adding files<tt>(e.g. screencast): </tt><a href="https://sourceforge.net/apps/trac/sourceforge/wiki/Release%20files%20for%20download" target="_blank">https://sourceforge.net/apps/trac/sourceforge/wiki/Release%20files%20for%20download</a>

Express-C:  <a href="http://www-01.ibm.com/software/data/db2/express/" target="_blank">http://www-01.ibm.com/software/data/db2/express/</a>

Source code for ibm_db2:  <a href="http://pecl.php.net/package/ibm_db2" target="_blank">http://pecl.php.net/package/ibm_db2</a>

Debugging PHP:  PDT2 (Eclipse for PHP) <a href="http://www.eclipse.org/pdt/downloads/" target="_blank">http://www.eclipse.org/pdt/downloads/</a> and install either XDebug or ZendDebug and configure in Apache and Eclipse.