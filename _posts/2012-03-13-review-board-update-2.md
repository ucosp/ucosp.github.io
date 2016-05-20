---
id: 2869
title: Review Board Update
date: 2012-03-13T09:46:35+00:00
author: rtholmes
layout: post
guid: http://ucosp.ca/?p=2869
permalink: /winter-2012/2012/03/review-board-update-2/
categories:
  - Winter 2012
---
Wei Lu Liu [writes](https://reviewboardstudents.wordpress.com/2012/03/13/ucosp-blog-post-march-12-2012/):

My name is Wei Lu Liu. I joined the Review Board team this semester as an undergraduate computer science student from Simon Fraser University. Gaining some open source development experience is what drove me at first, but being part of Review Board is far more than this. Throughout our development, we employ

&#8211; Git for revision control

&#8211; Google Groups/Code/Wiki/Blog for administration and reporting

&#8211; IRC/PasteBin for instant Q&A and discussing

&#8211; Review Board !!

Here comes the unique and interesting experience about working on Review Board: we are using Review Board itself in our development, which gives us first-handed feelings and feedback. With the “free” feedback, we can make Review Board better satisfy the developers as well as ourselves. With the goal of making our own lives easier, everyone in the team seems to have great interest and motivation.

So far I have had my hands on three bugs or projects. I would like to discuss my experience about each of them.

*  Adding “confirm password” fields to Review Board installation

The Review Board installation process has a couple of pages that ask the user to enter a new password, but the users do not have the chance to confirm their password. This project is a little different from others, as it is majorly about PyGtk. Without a whole understanding of PyGtk, I got stuck right after I added the “confirm password’ fields to the pages. I was trying to find some functions in that page class that validate the new field. I spent several hours but was still blocked. It is lucky that my mentor pointed out that the validation should be a widget. It turned out he was right, and we quickly worked it out.

This small  bug fix taught me that the Review Board is a quite big project that utilizes many third party packages like PyGtk. Although I considered myself good at Python, it is far from enough to handle the whole project.

* Tracking the users that change the review request

This project is about the product itself. It covers most of the main features of Django. The first thing I was faced with was to alter the database, more specifically, to add new fields to the tables to store the information and alter the restrictions and relations among the fields and tables. Django abstracts a table as a class, but adding a field to the table does not simply equal to adding a variable to the class. We have to make it happen to the real database using a tool called Django Evolution. I got stuck here again. I tried many tutorials online but just could not make it work. After consulting our mentors, I solved the problem and found that it was because I wrongly understood what Git does. In our case, Git only controls the source file types such as .py/.html/.js. The database file, .db typed, is not in its charge. So when I switched between branches the database file stayed the same. I learned that the details are important; I need to get more familiar with these software development concepts.

Altering the database successfully made it possible for me to quickly realize the user tracking features.I thought the project was about to finish, until our mentors raised some concerns: what if multiple users are making changes to the same review request? Whose change gets published? This is the famous race problems in transaction control. We decided to have a banner to tell the user not to confirm if there was another user editing the same page. This experience taught me that testing is so important in software development. Without the help from my mentors, I may think I was done with the project. Review Board has a unit test for every app, running and analyzing them is extremely import if I want high quality work. I was quite interested in those test cases and would see if I could learn writing some by myself.

* Weekly email updates

“Finding out what’s been happening on Review Board isn’t always easy. It might be worthwhile to have users be able to opt-in to weekly email updates from Review Board that tell them useful things about the groups that they belong to.” This is the idea why we want this feature. Django actually has really good email support. Review Board extends it and have specifically customized email methods itself. You should have realized that this project is more of administration level. I will write an admin command to realize it. I am just starting with it, and it looks interesting for me.

It is only one month left in this semester. I feel that I wasted a lot of time when I got stuck. I thought too much but did not ask enough questions. I have the shortcoming that I always want to have some basic idea before I ask questions. However, it usually turns out that I can not even have correct basic ideas if I just keep thinking and not asking, since the industry project is way more complex than the academic projects we do at school. Fortunately I have really helpful and friendly mentors and students in our team. After asking a couple of stupid questions, I got myself more familiar with the whole project. Now I can ask more meaningful questions after some self-exploration at first.

I am really grateful to UCOSP. I think it is a really good program for undergraduates. I did some internships before, but I felt that I could learn so little about the details of software development there. The internship employers, at least in my case, tend to put us on the works that are less risky for us to do. After all, they have too many things to consider, and we usually could not learn as much as we want. The UCOSP program is different, since everyone in the team have the same interest and goal: to learn and to contribute. In our case, the Review Board, if we can make it a better tool, it would be for the benefit of all the developers using it. Due to this reason, I think UCOSP is a really good program that compliments our academic and internship experience. I hope this program can continue evolving and benefiting more and more students.

Cheers,

Wei Lu Liu (Willer)