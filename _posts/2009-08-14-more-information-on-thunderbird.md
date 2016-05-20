---
id: 40
title: More Information on Thunderbird
date: 2009-08-14T12:58:15+00:00
author: Greg Wilson
layout: post
guid: http://ucosp.wordpress.com/?p=40
permalink: /2009-2010/thunderbird/2009/08/more-information-on-thunderbird/
categories:
  - Thunderbird
---
From [Blake Winton](http://bwinton.latte.ca/), the main technical contact for the Thunderbird project:

For this term, I think students will be working on a Django (Python) site to manage the ISP configuration information for Thunderbird. There may also be some Javascript work to hook in to whatever pieces need to be added to the database.

To quote [David Ascher](http://ascher.ca/blog/) (who&#8217;s in charge of Mozilla Messaging):

> From a student project POV, especially given the schedule (fall, when we&#8217;ll be locking things down in TB3), I suspect getting them working on the Django site that powers the database that manages the autoconfig data would be an interesting idea. Easier ramp up curve (a fairly straightforward Django app), some interesting problems (distributing trust, auditable records, email security).

Next term, there will probably be something to make the database more decentralized, which would be largely javascript-powered. (Basically check for the configuration values in places like &#8220;http://autoconfig.domain.com/mail.xml?domain=domain.com&#8221; for an email address of &#8220;me@domain.com&#8221;, and then fall back to the Mozilla Messaging servers if that doesn&#8217;t exist.

To quote David again:

> We&#8217;re also happy (likely after TB3, so maybe in a student project) to consider something more decentralized, so that an ISP (or meta-ISP like TUCOWS) could themselves manage the data storage based on some agreed upon domain, kinda like the Exchange autodiscovery model (but simpler =).