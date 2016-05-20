---
id: 2873
title: Review Board Update
date: 2012-03-26T21:58:51+00:00
author: rtholmes
layout: post
guid: http://ucosp.ca/?p=2873
permalink: /2009-2010/uncategorized/2012/03/review-board-update-3/
categories:
  - Uncategorized
---
Steven MacLeod [writes](http://reviewboardstudents.wordpress.com/2012/03/26/ucosp-blog-post/):

My experience with UCOSP has been very fulfilling thus far. I’ve met a lot of great people, and have enjoyed working on the Review Board project more than I ever would have expected. One of my favourite aspects of the program is the feeling that your contributions are significant; The code you write is distributed to and executed by real users. This is in stark contrast to the usual work which is done in university.

UCOSP gives you the chance to work on some really interesting projects, and I’d like to give on overview of what I’ve been working on thus far.

#### Review Bot:

The main project I’ve taken on for UCOSP is something I’ve dubbed “Review Bot”. The goal of Review Bot is to automatically execute static analysis tools on code that has been posted for review on Review Board. Basically, it will review code using external programs, and then post any issues it finds to Review Board.

Thinking through the design, and receiving feedback from the community looking to automate static analysis using Review Board, I came up with a plan of attack. My initial aspirations for Review Bot are illustrated below:

<div id="attachment_1577" class="wp-caption aligncenter" style="width: 610px;">
  <p>
    <a href="http://reviewboardstudents.files.wordpress.com/2012/03/reviewbot1.png"><img class="size-full wp-image-1577" title="Imagined Review Bot" src="http://reviewboardstudents.files.wordpress.com/2012/03/reviewbot1.png?w=600&h=514" alt="Review Bot of my dreams" width="600" height="514" /></a>
  </p>
  
  <p class="wp-caption-text">
    How Review Bot was envisioned &#8211; Warning: Imagination Required
  </p>
</div>

Yeah, that’s a code reviewing, go-go-gadget armed robot with a jet-pack. It reviews code written in any language, and can solve the halting problem. I considered allowing it to review its own code, but the risk of it becoming sentient and enslaving the human race was too great. But in all seriousness, I planned to make a highly versatile code reviewing bot, which other developers could extend to support the static analysis tools of their liking.

However, it can be hard to properly scope a project when dealing with an unfamiliar code base. I quickly realised this as I ventured deeper into Review Board’s API and extension support. Once I’d begun working through the implementation of Review Bot, it became apparent that my project was going to be a lot of work! Review Board lacked some of the features necessary to support the Review Bot I had envisioned. My first order of business was to fix this; I set out to extend the Web API and expand the feature set of the extension system.

Review Board’s extension system is powerful, young, and light in the documentation department. The lack of online documentation was a little worrisome at first, but prior developers had commented their code very well. Combine this with some very knowledgeable and helpful mentors, and hacking on extensions proved to be a blast. Even though Review Board is a mature code base, I was able to work on something fresh and exciting; you don’t have to worry about backwards compatibility when the feature isn’t in use yet. My time spent with the extension system has given me the expertise needed to document it, and my beginner’s guide for future developers is nearing completion.

All this related development has kept Review Bot on the back-burner for a lot of the term. To give you an idea of Review Bot’s current state, here is an artists rendering of the progress I’ve made:

<div id="attachment_1578" class="wp-caption aligncenter" style="width: 610px;">
  <p>
    <a href="http://reviewboardstudents.files.wordpress.com/2012/03/reviewbot2.png"><img class="size-full wp-image-1578" title="Current State of Review Bot" src="http://reviewboardstudents.files.wordpress.com/2012/03/reviewbot2.png?w=600&h=514" alt="What Review Bot can accomplish at the moment" width="600" height="514" /></a>
  </p>
  
  <p class="wp-caption-text">
    What Review Bot can accomplish at the moment
  </p>
</div>

All right, I might be selling myself a little short with that picture. While it is true that Review Bot can’t actually analyse any code yet, progress should be quick now that Review Board has the features needed to support it. By the end of the term Review Bot should be automatically analysing Python code with the pep8 style checker. Some features, such as allowing tools to analyse the entire code base and not just the modified files, had to be dropped – but I’m still happy with how the final product will look.

#### In Closing:

I really can’t stress how happy I am to be participating in this program, and I recommend it to any students given the opportunity to participate. I’d like to thank the UCOSP steering committee for organizing everything. Also, a very big thank you to the Review Board mentors: Christian Hammond, David Trowbridge, and Mike Conley. These guys have made this experience awesome, and I really appreciate all the time and effort they have committed to the program.

Thanks for bearing with my artistic “ability”,

Steven MacLeod