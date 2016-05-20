---
id: 2776
title: 'Fall semester code sprint — it&#8217;s a wrap!'
date: 2010-10-04T15:01:16+00:00
author: Andrew Louis
layout: post
guid: http://ucosp.ca/?p=2776
permalink: /fall2010/2010/10/ucosp-code-sprint/
categories:
  - Fall 2010
tags:
  - Code Sprint
---
This weekend, over 50 students and project mentors gathered in Toronto for this semester&#8217;s code sprint.

[<img class="alignnone size-full wp-image-2782" title="IMG_6460" src="http://ucosp.ca/wp-content/uploads/2010/10/IMG_6460.jpg" alt="" width="610" srcset="http://ucosp.ca/wp-content/uploads/2010/10/IMG_6460.jpg 846w, http://ucosp.ca/wp-content/uploads/2010/10/IMG_6460-300x198.jpg 300w" sizes="(max-width: 846px) 100vw, 846px" />](http://ucosp.ca/wp-content/uploads/2010/10/IMG_6460.jpg)

Why go through all the trouble and expense of bringing students together to a single physical location to work on their projects? Isn&#8217;t the point of UCOSP to teach students to work in a distributed environment? Yes, but from experience, we&#8217;ve found that when teams are able to meet even once, the odds of success are dramatically increased.

For many, remotely collaborating with teammates, a mentor, or mailing list is intimidating, especially for the many students who&#8217;ve never worked in a distributed fashion before. Getting together at the code sprint leads to smoother interactions in the future. It&#8217;s also a great chance to meet other students and industry contacts.

[<img class="size-full wp-image-2778 alignnone" title="IMG_6502" src="http://ucosp.ca/wp-content/uploads/2010/10/IMG_6502.jpg" alt="" width="610" srcset="http://ucosp.ca/wp-content/uploads/2010/10/IMG_6502.jpg 846w, http://ucosp.ca/wp-content/uploads/2010/10/IMG_6502-300x200.jpg 300w" sizes="(max-width: 846px) 100vw, 846px" />](http://ucosp.ca/wp-content/uploads/2010/10/IMG_6502.jpg)

The code sprint also marks the point in the semester where students decide on goals for the remaining two months of the semester. Now that environments are set up and the code bases are explored, students can now move forward and accomplish a meaningful chunk of work.

[<img class="alignright size-medium wp-image-2779" title="IMG_6490" src="http://ucosp.ca/wp-content/uploads/2010/10/IMG_6490-300x200.jpg" alt="" width="300" height="200" srcset="http://ucosp.ca/wp-content/uploads/2010/10/IMG_6490-300x200.jpg 300w, http://ucosp.ca/wp-content/uploads/2010/10/IMG_6490.jpg 846w" sizes="(max-width: 300px) 100vw, 300px" />](http://ucosp.ca/wp-content/uploads/2010/10/IMG_6490.jpg)

From Friday morning (apologies to our Pacific Standard Time students!) until Sunday noon, students got remaining environment kinks sorted out, discussed tools and strategies for their projects, negotiated scope, and began their work on their goals. After these two and a half days of work, what got done?

**[POSIT](http://posit.hfoss.org/)** (Portable Open Search and Identification Tool) ****is a mobile app for the Android platform that enables disaster relief workers to capture and send back _finds_ from the field_._ Besides being able to play around with the application on handsets that mentor Ralph Morelli brought along, the team fixed some outstanding bugs (and found some new ones) and submitted their first patches. They also scoped out tasks for the remainder of the semester.

**[Ingres](http://ingres.com/)** is an open-source relational database; the team will be focusing on the [geospational components](http://community.ingres.com/wiki/IngresGeospatial). With its four million lines of code and years of development, the biggest challenge for students was setting up a working build environment. With this hurdled cleared, the focus for the next two months will be adding different output formats and working on documentation and testing.

[<img class="alignright size-medium wp-image-2780" title="IMG_6479" src="http://ucosp.ca/wp-content/uploads/2010/10/IMG_6479-300x200.jpg" alt="" width="300" height="200" srcset="http://ucosp.ca/wp-content/uploads/2010/10/IMG_6479-300x200.jpg 300w, http://ucosp.ca/wp-content/uploads/2010/10/IMG_6479.jpg 846w" sizes="(max-width: 300px) 100vw, 300px" />](http://ucosp.ca/wp-content/uploads/2010/10/IMG_6479.jpg)

[**Basie on Pinax**](http://blog.basieproject.org/)&#8216;s goal is to take components of Basie, a web-based software project forge, and rebuilding them on top of Pinax, a collection of reusable apps for Django. With a version control application almost finished, the next goal will be adding a mailing list feature to Pinax. Over the weekend, the team went from nothing to &#8220;we can send mail!&#8221; and will be tackling access control features next. You can follow the group&#8217;s [progress on their blog](http://blog.basieproject.org/).

The **[Freeseer](http://fosslc.org/drupal/freeseer)** project produces a video capture utility capable of capturing presentations. Over the weekend, the team almost finished a new internationalization component and fixed some filesystem-related bugs. Next up: adding live streaming support and packaging the project for different Linux distributions.

The [**fab4browser**](http://code.google.com/p/fab4browser/) is a tool to collaboratively annotate files and there is a demand to gather and display analytics. Since this team&#8217;s project isn&#8217;t quite on the fab4browser project but a tool that uses it, the first task was coming up with a new name. The team settled on &#8220;CORAL&#8221;, short for &#8220;collaborative review analysis of literature.&#8221; Over the weekend, the team picked the tools that they&#8217;ll be using, tested visualization tools, and divided up the future work between the PHP back-end, the middle tier, and the visualization functionality.

[<img class="alignright size-medium wp-image-2777" title="IMG_6680" src="http://ucosp.ca/wp-content/uploads/2010/10/IMG_6680-300x173.jpg" alt="" width="300" height="173" srcset="http://ucosp.ca/wp-content/uploads/2010/10/IMG_6680-300x173.jpg 300w, http://ucosp.ca/wp-content/uploads/2010/10/IMG_6680.jpg 846w" sizes="(max-width: 300px) 100vw, 300px" />](http://ucosp.ca/wp-content/uploads/2010/10/IMG_6680.jpg)

**[Review Board](http://www.reviewboard.org/)** is a powerful web-based tool designed to &#8216;take the pain out of code review.&#8217; On the weekend, the team worked on integrating the post-commit workflow, solidifying the third-party extension framework, and shiny new tools for using the new web API. Future projects include work on an easy-to-use Windows installer, and usability updates to the web interface. You can follow their progress [on the team blog](http://reviewboardstudents.wordpress.com/).

[**Markus**](http://markusproject.org/) is a grading and code review tool that gives the flexibility of pen-on-paper marking through the web. One week before the code sprint, the Markus project was [moved over to Github](http://github.com/MarkUsProject/Markus) so part of the code sprint weekend was spent on adjusting to the new git workflow. Students also fixed some bugs and made their first patches. Sub-groups will be working on the two goals for this semester: adding an automated testing framework (students can run tests on their code; instructors can automatically test submissions) and building report generation tools. You can follow their progress on [the team&#8217;s blog](http://blog.markusproject.org/).

The **[Technology Explorer for IBM DB2](http://sourceforge.net/projects/db2mc/)** is a web-based tool that is a teaching tool for users new to DB2. This weekend was the first real chance to really play around with the codebase and the team was able to finish a few small projects. For the remainder of the semester, they&#8217;ll be working on some requests that came from the project&#8217;s users: improving the tool&#8217;s scripting language and adding reporting and exporting functionality

<p style="text-align: center;">
  <a href="http://ucosp.ca/wp-content/uploads/2010/10/IMG_6464.jpg"><img class="aligncenter size-full wp-image-2781" title="IMG_6464" src="http://ucosp.ca/wp-content/uploads/2010/10/IMG_6464.jpg" alt="" width="610" srcset="http://ucosp.ca/wp-content/uploads/2010/10/IMG_6464.jpg 846w, http://ucosp.ca/wp-content/uploads/2010/10/IMG_6464-300x200.jpg 300w" sizes="(max-width: 846px) 100vw, 846px" /></a>
</p>

### And a word from our sponsors

Without sponsor support, doing a code sprint with all UCOSP students would be impossible. Thanks again to Google, O&#8217;Reilly, the Canadian Association of Computer Science Chairs, the Jonah Group, and Research in Motion for your support!