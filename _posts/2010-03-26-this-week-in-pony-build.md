---
id: 2688
title: 'This week in Pony-Build&#8230;'
date: 2010-03-26T05:37:44+00:00
author: kshakyaz
layout: post
guid: http://ucosp.wordpress.com/2010/03/26/this-week-in-pony-build/
permalink: /2009-2010/uncategorized/2010/03/this-week-in-pony-build/
categories:
  - Uncategorized
---
During our last conference call we talked about where everybody was and what problems we were facing. Here are the notes from the last conversation.

**pony-build conference call notes / from, mar15, 2010; updated mar 22, 2010;******

**Khushboo:**

&#8211; build-nose is still in a very old master that is incompatible with mine; could you copy just that file over to a clean checkout of my master, add/commit,

push back to github, and let me know where?

&#8211; .pony-build cachedir creation?

&#8211; mechanize?

<http://kshakyaz.wordpress.com/>

[](http://kshakyaz.wordpress.com/)**Max:**

&#8211; has been &#8220;chipping away at small things&#8221;.  working on create\_cache\_dir, pip failure, letc.

&#8211; testing timeouts; switch to using signal.alarm?

<http://docs.python.org/library/signal.html> <&#8211; Rose will look at this

Most signal methods not available under windows. :/ (rose)

&#8211; will look at adding failure flag to context, and modifying &#8216;do&#8217; to be context-failure-aware for e.g. pip

failure

<http://mlaite.blogspot.com/>

**Fatima:**

&#8211; working with mercurial branches; status update?

<http://cherkf.wordpress.com/>

**Jack:**

&#8211; response? status update?  continuing work with pony-client rework, going off Titus&#8217; latest suggestions, continuing work tomorrow

<http://jackcarlson.wordpress.com/>