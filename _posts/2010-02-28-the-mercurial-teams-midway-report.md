---
id: 2428
title: 'The Mercurial Team&#039;s Midway Report'
date: 2010-02-28T04:33:41+00:00
author: Benjamin
layout: post
guid: http://ucosp.wordpress.com/?p=2428
permalink: /2009-2010/mercurial/2010/02/the-mercurial-teams-midway-report/
categories:
  - Mercurial
---
When we set out at the beginning of UCOSP, my goal was for us to contribute significantly to Mercurial by the end of the semester. How well have we accomplished that goal so far?

At the beginning of the semester, all of the students were given small, self-contained bug fixes and features that we&#8217;d discovered people wanted over the course of developing Kiln, mostly in the form of Mercurial extensions. Four of these were quickly completed: [cedit](http://bitbucket.org/paulitex/cedit/), a command-line-based way to configure Mercurial; [cache-annotations](http://bitbucket.org/antmar/cache-annotations/), which makes annotating files repeatedly ridiculously fast; globexclude, which allows you to exclude files based on their glob pattern when doing conversions to Mercurial; and [caseguard](http://bitbucket.org/alexandru/caseguard/), which warns you when you are committing files that have names that will prevent Mac and Windows users from using your repository. Of these, globexclude and caseguard will be submitted (with some slight modifications) for inclusion into Mercurial 1.6, and cache-annotations already ships with every version of Kiln. This part of the project I consider a complete success.

Since then, we have transitioned from everyone doing a little project to everyone working on [bfiles](http://vc.gerg.ca/hg/hg-bfiles), an extension to Mercurial that is designed to ameliorate using Mercurial with projects that involve large binary files.

I would be lying if I said I wasn&#8217;t slightly disappointed with the work done on bfiles so far—not really through any fault of my students, as much as due to the nature of what they&#8217;re trying to accomplish. bfiles is necessarily a more complex problem than the initial, self-contained feature sprints: bfiles requires some changes to Mercurial&#8217;s workflow, and these changes don&#8217;t always have a single, straightforward solution, and so everyone has to take the discussion to the Mercurial mailing list to figure out how to proceed. Having these discussions is unquestionably _not_ a waste of time. These are delicate issues, and working with the Mercurial community to determine how to proceed is an absolutely necessity. This has, unfortunately, had the side-effect of delaying writing some of the code we wanted for bfiles until we can get some of the design straightened out.

I&#8217;m nevertheless still very optimistic for the second half of the semester. We&#8217;ve sorted out a lot of the hard issues, allowing everyone to begin focusing on writing code again (even if only for initial prototypes, in some cases). Simultaneously, we&#8217;ve begun working on some aspects of bfiles that do not require so much debate to ensure that we&#8217;re doing the &#8220;right&#8221; thing. This means we can continue to code, while still carefully consulting the community on ambiguous areas.

Balancing requirements gathering with simply getting the code done can be a complicated affair on open-source and commercial projects alike. I think we&#8217;ve been erring too much towards discussion in the last couple of weeks, but as long as we can correct ourselves soon and get focused on the code again, I&#8217;m still confident that we&#8217;ll get nearly everything accomplished this semester that we set out to do.