---
id: 2199
title: Mercurial Progress Report (Week 4)
date: 2010-01-29T16:09:03+00:00
author: Anton Markov
layout: post
guid: http://ucosp.wordpress.com/?p=2199
permalink: /2009-2010/mercurial/2010/01/mercurial-progress-report-week-4/
categories:
  - Mercurial
  - Status
---
We have made substantial progress towards getting our initial contributions ready for submitting to the mercurial-devel mailing list. This has been a week of testing and code reviews where we all learned something new about Mercurial and writing python code in general.

To summarize, you can expect the following extensions to be submitted to the mercurial mailing list in the next week:

  * tagmerge (wendyY): support smart merging of tag files (tags are labels for specific commits or heads) 
      * some fixes and testing, testing, testing
  * cedit (paulitex): command line and interactive editing of mercurial configuration files with shortcuts for common setup operations 
      * submitted iniparse (external lib) changes upstream
      * documentation, bootstrapping, testing, testing, testing
  * convert (Tessa): modifying the convert extension to support wildcards in exclude statements 
      * order/precedence of include vs. exclude
  * cache-annotations (antmar): cache the results of the annotate (blame) command to speed up generation of annotations at future revisions. 
      * case-insensitive cache store
      * code reviews
  * caseguard (alexandru): warn/prevent users from committing files which cause problems on case-insensitive systems 
      * code reviews
      * finishing up support for guarding specific commands

We posted our detailed progress reports on the [January 28&#8217;th wiki page](https://ucosp.fogbugz.com/default.asp?W12 "January 28 progress reports") before this week&#8217;s meeting.

As we discussed last week, our next project is to improve support for binary files in Mercurial.

  * Binary files (or large text files) are often replaced with completely new versions during a commit. As a result they don&#8217;t compress well using deltas, and we end up storing many copies of the file, taking up space in each copy of the repository.
  * One solution is to store the files in a centralized store (local or remote) which is shared by many copies of the repository.
  * This solution is currently implemented as the &#8216;bfiles&#8217; extension by Greg Ward. It provides commands for dealing with b-files that mirror standard Mercurial commands (ex. &#8216;hg bfstatus&#8217; vs. &#8216;hg status&#8217;).
  * We plan to integrate bfiles with existing mercurial commands, add full support for HTTP-based stores, and other improvements.

Everyone has had a chance to read about and play with bfiles over the past week. The Waterloo people (Tessa, wendyY, and I) have decided to tackle integration with existing Mercurial commands.