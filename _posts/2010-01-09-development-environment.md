---
id: 1954
title: Development Environment
date: 2010-01-09T23:20:24+00:00
author: evanstratford
layout: post
guid: http://ucosp.wordpress.com/?p=1954
permalink: /2009-2010/thunderbird/2010/01/development-environment/
categories:
  - Thunderbird
---
I&#8217;ve gone through the motions [here](https://developer.mozilla.org/en/Simple_Thunderbird_build) and [here](https://developer.mozilla.org/en/Incremental_Build), but that only gets you so far; comm-central is _massive_, so some additional tools are in order. Here&#8217;s what I&#8217;m using so far:

  * the MXR search tool ([comm-central here](http://mxr.mozilla.org/comm-central/search)) to perform rgrep-style queries on the codebase. (A REST API here would be useful, I suspect&#8230;)
  * exuberant-ctags in vim, following setup 3 as described [here](http://ctags.sourceforge.net/faq.html#15). (Building the tag files takes roughly 15 minutes on my laptop.)
  * a pair of bash aliases to switch between debug and release .mozconfigs.
  * [this list](http://mercurial.selenic.com/wiki/GitConcepts), which provides a rough mapping between hg and git commands.

Hopefully this will save someone time 🙂

In the spirit of reciprocity: anyone else have suggestions for links, tools, etc. that could speed up the learning/working process? (Although I&#8217;ve placed this under the Thunderbird category, general feedback is more than welcome!)