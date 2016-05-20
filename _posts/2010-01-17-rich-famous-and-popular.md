---
id: 2049
title: Rich, Famous, and Popular
date: 2010-01-17T15:35:28+00:00
author: Greg Wilson
layout: post
guid: http://ucosp.wordpress.com/?p=2049
permalink: /2009-2010/education/2010/01/rich-famous-and-popular/
categories:
  - Education
---
Almost everyone who joins a new project says it sooner or later: &#8220;More documentation, please.&#8221; No one can make sense of 30,000 lines of code in one gulp: everyone wants an overview or roadmap to help them make sense of things. So why don&#8217;t they exist?

  1. Almost by definition, by the time you can _write_ that document, you don&#8217;t need it yourself. You probably also have a dozen tickets assigned to you by then too, all of which really, really need to be fixed for next week&#8217;s release.
  2. Overviews are much harder to write than lower-level Javadoc-style explanations of what individual methods do. The latter is just an assemblage of facts; the former requires story-telling skills, and good storytellers are rare in any field (not just programming).
  3. Anyone who ever _has_ written an overview document knows that it will rust pretty quickly. Design decisions will change, code will be refactored, and pretty quickly, that 30-page tutorial you sweated over is so far out of date that it&#8217;s actually doing as much harm as good. Keeping it up to date is a never-ending struggle, and it&#8217;s not like people have stopped assigning you tickets&#8230;

Jacob Kaplan-Moss (from the Django team) wrote a good post a while back about [writing great documentation](http://jacobian.org/writing/great-documentation/). It&#8217;s worth reading, and he&#8217;s right: after a certain point, investing effort in documentation and discussion actually pays a bigger dividend for open source projects than investing effort in code. It&#8217;s still an open research problem, though; anyone who ever figures out how to generate, check, and update narrative explanations of how code is structured, what it does, and (most importantly) why, will be rich, famous, and popular. Lemme know how it goes&#8230;