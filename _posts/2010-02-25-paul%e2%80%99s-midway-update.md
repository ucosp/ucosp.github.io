---
id: 2395
title: Paul’s Midway Update
date: 2010-02-25T23:12:31+00:00
author: paulitex
layout: post
guid: http://ucosp.wordpress.com/?p=2395
permalink: /2009-2010/uncategorized/2010/02/paul%e2%80%99s-midway-update/
categories:
  - Uncategorized
---
I&#8217;m pretty happy with both my progress so far and the progress of our entire team (Mercurial). As Anton and Tessa have mentioned, we hit a bit of a slow period recently with bfiles but I think that&#8217;s natural. We had an exceptionally productive first month and a bit (largely thanks to the code sprint!). Every person on our team contributed non-trivial extensions that tangibly increased the usability of Mercurial. I think that is something we should be very proud of.

Personally, I wrote an editor for Mercurial configuration files that works both off the command-line and in interactive mode to safely and easily manage configurations. The standard way to edit configuration files currently is manually with a text editor. Some people find this tedious or intimidating &#8211; it is definitely more error prone than an custom editor. I announced &#8216;cedit&#8217; on the mercurial mailing list a few weeks ago, and I&#8217;m not sure how many people are using it but I know I am regularly so at least one person is benefiting from my work ;). If you are using Mercurial and want to try it out, you can get it [here](http://bitbucket.org/paulitex/cedit/)

The last couple weeks we&#8217;ve all been coming to grips with bfiles. I&#8217;ve finally found a sub-project that I&#8217;m pretty excited about tackling. It is an extension to bfiles (which is in turn is an extension to Mercurial) that adds a single command: bfilesify (and possibly unbfilesify, if things go well). The idea is it takes an existing Mercurial repository a clones it to a new one that is identical, except for every file that should be managed by bfiles is. The result should be that the second repository is (often) vastly smaller than the original. Moreover, it allows people to try out bfiles immediately &#8216;for free&#8217; which should really up adoption rate of bfiles among Mercurial users.

So I&#8217;m excited about taking on bfilsify for the second half of the semester. If UCOSP part 1 to me is cedit and part 2 is bfilesify (and they turn out well and at least a couple people use them) I will definitely consider UCOSP a success.