---
id: 2940
title: Initial UCOSP Report
date: 2014-02-21T15:10:41+00:00
author: rtholmes
layout: post
guid: http://ucosp.ca/?p=2940
permalink: /winter-2014/2014/02/initial-ucosp-report/
categories:
  - Winter 2014
---
<p class="c5">
  <span>Hi! My name is Brandon Noad, and I am a Computer Science student at the University of Waterloo. This term I was selected to participate in the </span><span class="c0"><a class="c1" href="http://ucosp.ca/">UCOSP program</a></span><span> where I get to work on an open source software project with other students from around the globe—for credit!</span>
</p>

<p class="c6 c5">
  The project I was assigned to is called GeoTrellis. GeoTrellis is a <span class="c0"><a class="c1" href="http://www.scala-lang.org/">Scala</a></span> library and framework for creating useful, high performing web services that load and manipulate <span class="c0"><a class="c1" href="http://geotrellis.github.io/glossary/#raster_data">raster data</a></span> (visit the GeoTrellis <span class="c0"><a class="c1" href="http://geotrellis.github.io/index.html">documentation</a></span> and <span class="c0"><a class="c1" href="https://github.com/geotrellis/geotrellis">GitHub</a></span> pages for more information). You can check out a cool example of GeoTrellis in action <span class="c0"><a class="c1" href="http://demo.geotrellis.com/chatta/">here</a></span>.
</p>

<p class="c6 c5">
  In the past few months, I have completed Coursera’s “<span class="c0"><a class="c1" href="https://www.coursera.org/course/progfun">Functional Programming Principles in Scala</a></span>” course, written a web application in Scala using the <span class="c0"><a class="c1" href="http://www.playframework.com/">Play</a></span> framework, and attended several local <span class="c0"><a class="c1" href="http://www.meetup.com/WaterlooScala/">Scala Meetups</a></span> here in Waterloo. I really enjoy programming in Scala, and GeoTrellis was at the top of my list of project choices because I wanted to continue to improve my Scala programming skills. Although I had very little experience working with geospatial data, I was able to get up to speed quickly with help from my project mentor <span class="c0"><a class="c1" href="https://github.com/lossyrob">Rob</a></span>.
</p>

<p class="c6 c5">
  To prepare for the UCOSP Winter 2014 code sprint, I completed the following list of tasks:
</p>

<ul class="c7 lst-kix_ylhsgqvhxe5q-0 start">
  <li class="c2">
    <span>Forked the GeoTrellis repository (</span><span class="c0"><a class="c1" href="https://github.com/BrandonNoad/geotrellis">my fork</a></span><span>).</span>
  </li>
  <li class="c2">
    <span>Built the project using </span><span class="c0"><a class="c1" href="http://www.scala-sbt.org/">sbt</a></span><span> and ran the unit tests.</span>
  </li>
  <li class="c2">
    <span>Submitted a </span><span class="c0"><a class="c1" href="https://github.com/geotrellis/geotrellis/pull/700">pull request</a></span><span> to fix a typo in the README.</span>
  </li>
  <li class="c2">
    <span>Created a </span><span class="c0"><a class="c1" href="https://github.com/BrandonNoad/geotrellis/blob/GeoTrellis-Assignment/src/test/scala/geotrellis/GeoTrellisAssignment.scala">new test file</a></span><span> containing a FunSpec test with ShouldMatchers that runs a single unit test. This test creates an Array of 100 random integers, sorts the array, and checks to make sure that for every i, j in {0 &#8230; 99}, if i < j, then array[i] < array[j], where array[x] represents the xth element in the sorted array.</span>
  </li>
  <li class="c2">
    <span>Completed the GeoTrellis </span><span class="c0"><a class="c1" href="http://geotrellis.github.io/tutorials/webservice.html">web service tutorial</a></span><span>.</span>
  </li>
  <li class="c2">
    <span>Worked on one of the project’s issues (</span><span class="c0"><a class="c1" href="https://github.com/geotrellis/geotrellis/issues/678">#678</a></span><span>).</span>
  </li>
  <li class="c2">
    <span>Submitted a </span><span class="c0"><a class="c1" href="https://github.com/geotrellis/geotrellis/pull/729">pull request</a></span><span> to fix issue #678.</span>
  </li>
  <li class="c2 c8">
    <span>Read chapters 1-15 of “</span><span class="c0"><a class="c1" href="http://www.artima.com/pins1ed/">Programming in Scala</a></span><span>”.</span>
  </li>
</ul>

<p class="c3 c6">
  This term’s code sprint took place at <span class="c0"><a class="c1" href="https://www.facebook.com/pages/Facebook-HQ/166793820034304">Facebook HQ</a></span> in Menlo Park, CA. It was my first time in California, and although California is supposedly in the midst of a <span class="c0"><a class="c1" href="http://www.news10.net/story/news/local/2014/02/10/obama-to-visit-drought-stricken-california/5377073/">drought</a></span>, it rained for most of the weekend. That said, I was just happy to escape the <span class="c0"><a class="c1" href="http://globalnews.ca/news/1100134/polar-vortex-refuses-to-leave/">polar vortex</a></span>, so I wasn’t going to let a bit of rain ruin my trip. At the sprint, I had the opportunity to meet my project mentor, Rob, and the other students working on the project—Mitch (<span class="c0"><a class="c1" href="http://www.ubc.ca/">UBC</a></span>), Jonathan (<span class="c0"><a class="c1" href="http://web.mit.edu/">MIT</a></span>), and Armstrong (<span class="c0"><a class="c1" href="http://www.ubishops.ca/index.html">BU</a></span>). Overall, I had an amazing time. Besides coding alongside my teammates, I listened to a couple of engaging talks by <span class="c0"><a class="c1" href="http://scottchacon.com/about.html">Scott Chacon</a></span> and <span class="c0"><a class="c1" href="http://cs210.stanford.edu/about.html">Jay Borenstein</a></span> about GitHub and startups respectively, visited Stanford’s beautiful <span class="c0"><a class="c1" href="http://www.stanford.edu/dept/visitorinfo/tours/virtual/">campus</a></span>, ate a lot of beef jerky (<span class="c0"><a class="c1" href="http://goldenvalleynatural.com/beef/natural-beef-jerky-black-pepper.html">mmmmm</a></span>), bowled my first <span class="c0"><a class="c1" href="http://www.bowlluckystrike.com/three-strikes-turkey-origin">turkey</a></span>, and had a <span class="c0"><a class="c1" href="http://www.samovarlife.com/">cup of tea</a></span> in downtown San Francisco.
</p>

<p class="c3 c6">
  One of the challenges for the sprint was to identify an action plan for the rest of the term. My task is to implement a Scala wrapper for the <span class="c0"><a class="c1" href="http://www.vividsolutions.com/jts/jtshome.htm">JTS Topology Suite</a></span> that facilitates vector to raster operations. By using Scala language features such as <span class="c0"><a class="c1" href="http://www.scala-lang.org/old/node/123">sealed classes</a></span>, we can leverage the power of Scala’s type system to make working with <span class="c0"><a class="c1" href="http://geotrellis.github.io/glossary/">vector data</a></span> much more enjoyable for developers. Rob thinks that if we design and implement this wrapper well, it may become the “go-to” solution for working with vector data in Scala. Once the wrapper is complete, the next step is to create a <span class="c0"><a class="c1" href="http://geojson.org/geojson-spec.html#feature-objects">Feature</a></span> library on top of it to replace the <span class="c0"><a class="c1" href="http://geotrellis.github.io/overviews/vector.html">existing suite of vector operations</a></span> in the main GeoTrellis project. At the sprint, I began working on the wrapper and submitted a <span class="c0"><a class="c1" href="https://github.com/geotrellis/geotrellis/pull/734">pull request</a></span> after implementing intersection, union, and difference methods for the various geometry types. It’s exciting to be working on such a meaningful project.
</p>

<p class="c3 c6">
  The GeoTrellis team uses a fairly standard Git/GitHub workflow. We create topic branches off of master for the issues/features we are working on, and we commit to the topic branches locally as well as regularly push any work done to the same named branch in our forked GitHub repo. After hearing Scott Chacon speak at the sprint, Rob decided it would be a good idea to open pull requests as early as possible (e.g. after your first commit). These pull requests then act as a form of code review, allowing us to communicate and receive feedback about our work. Once our work has been reviewed and <span class="c0"><a class="c1" href="http://shipitsquirrel.github.io/">approved</a></span>, it can be merged into master.
</p>

<p class="c3 c6">
  To keep in touch with Rob and the rest of the team, we have a weekly <span class="c0"><a class="c1" href="http://www.extremeprogramming.org/rules/standupmeeting.html">standup meeting</a></span> via Google Hangouts. GeoTrellis also has an IRC channel (#geotrellis) on freenode and a <span class="c0"><a class="c1" href="https://groups.google.com/group/geotrellis-user">mailing list</a></span>.
</p>

<p class="c3 c6">
  If you have read this far and are still wondering if you should apply for UCOSP next term, the answer should definitely be yes! Meeting and interacting with the other students at the sprint was an amazing experience, and my confidence that I belong alongside other software developers has grown as a result. Having the opportunity to do version control, unit testing, and code reviews on a real-world software project has been an invaluable experience so far, and I am certain that my skills as a developer will continue to improve throughout the rest of the UCOSP program.
</p>