---
id: 2104
title: '&quot;What we learnt&quot; + &quot;Where we&#039;ll go&quot;'
date: 2010-01-19T15:12:35+00:00
author: clgoh
layout: post
guid: http://ucosp.wordpress.com/?p=2104
permalink: /2009-2010/ingres/2010/01/what-we-learnt-where-well-go/
categories:
  - Ingres
  - Sprint
tags:
  - Code Sprint
  - Ingres
  - Winter 2010
---
The day before the sprint, I knew of nothing about what I should do and what I can do in this project. I woke up at 5 on Friday morning, took a taxi to the bus terminal, got onto Greyhound to Toronto, got lost on our way to Bahen Centre (we were on University and College, 5 minutes away from Bahen, lol)  To my surprise, I arrived, and joined a team of people as lost as I was. We found out throughout the sprint, many differences between universities, the courses, the cultures, etc. But all of us being in our last year, I believe there&#8217;s one thing in common that we&#8217;ve learnt before we get there: Well, no one&#8217;s going to help us if we don&#8217;t start helping ourselves. Before long, the whole team started the sprint ourselves. We asked lots and lots of questions (Thank you very much Andrew for your detailed presentation and all your help even by having to whisper), we read wiki pages, downloaded source code and snorkeled in it. No one sat still waiting for an answer, there was no awkward silent moment as the team of &#8220;professionals&#8221; blended from the very first day and moved forward as one. The three days went by very quickly.

We learnt the following during the sprint:

&#8211; OpenLayers draws map using Web Mapping Service provided by Geoserver, which in turns uses Geotools to obtain GeoSpatial Data from databases. Geotools can currently talk to many databases but not Ingres.

&#8211; In Geotools there are connectivity code under modules/plugin/jdbc and modules/plugin that uses various jdbc implementations to connect to various databases. There is also a deprecated version of the framework scheduled to be removed soon. Ingres team needs to make a similar jdbc implementation under Geotools to add support for Ingres.

&#8211; Sara and Eva will be working on the Ingres server side to make sure GeoSpatial queries are handled properly, while Anthony, Henry, Xiaoxiao and Lim work on Geotools to add Ingres support.

We decided the following during the sprint:

The project lead will communicate with the team and with the community at large to keep everyone informed about the status of the team, and make sure the team is moving in the right direction. Lim will take on this role.

The high-level view of the project is:

&#8211; Study the code and play with Geotools in action

&#8211; Design and plan potential changes to Geotools source tree

&#8211; Implement the designs and also implement support for GeoSpatial data in Ingres

&#8211; Unit test the Ingres connectivity code in Geotools, test GeoSpatial data support in Ingres, and system test Geotools actually using Ingres.

Now everyone&#8217;s back to where they are from, but technology is constantly connecting us together. We are all a phone call/email/IM message away from each other, and we are preparing for the next get-together online every Monday with more progress to make.