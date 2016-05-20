---
id: 2972
title: Reflecting on UCOSP
date: 2014-12-07T21:18:28+00:00
author: rtholmes
layout: post
guid: http://ucosp.ca/?p=2972
permalink: /fall-2014/2014/12/reflecting-on-ucosp/
categories:
  - Fall 2014
---
<div class="page" title="Page 1">
  <div class="section">
    <div class="layoutArea">
      <div class="column">
        <p class="p1">
          Andrew Hong from the University of Toronto gives us his impressions of the program.
        </p>
        
        <p>
          It has been almost two full months in the Undergraduate Capstone Open Source Projects (UCOSP) program and now that I look back, it has been an amazing experience. If you are reading this, you probably have an idea of what the UCOSP program is about and are looking to find out more. UCOSP is basically where you get to work on a distributed open source project for a semester with a team of students and mentors. The mentors and students are likely from all over the country so do not expect to see them in person regularly. You will do most of your communication online with your team through whichever method is preferred; audio, video, text chat, etc. UCOSP is very different from your typical course, you work however you want, and whenever you want. There are deadlines to be met so it keeps everything and everyone in line. Expect to work about 8-10 hours per week and sometimes more, when it is necessary. You do not get any marks until the end of the course but you will receive feedback along the way so you know how you are doing in relation to your mentor’s expectations. You can always ask them how you are coming along just in case you think you are slacking. If there is one takeaway I want you to get out of reading this, it is: enroll into UCOSP now, you will not regret it!
        </p>
        
        <p>
          The code sprint this year was held at the Mozilla office in Toronto. It was a phenomenal and busy three days. We had all the students enrolled in UCOSP all in one space and separated into our respective teams. For ReviewBoard, we worked on bugs, started projects for the term and made sure everyone was on track. We, the students, were all set up with our environments so there was little time wasted there. It was an awesome experience to meet your fellow students and mentors so you can easily put a face to those internet nicknames that you are always chatting with 🙂 I believe the code sprint was crucial to UCOSP. It makes people familiar with who they are working with and thus making it a more comfortable working environment for all. Food and drinks were provided so no need to worry about thirst or hunger strikes. After hours was up to the team, we decided to wander around the city in search of good food and a good time. Since I was the only Toronto student in my team, I gave them a mini tour of the downtown core, without trying to be touristy. We went for hidden gems and not-so-typical dining spots and by the end of it all, it sounded like everyone had a great time!
        </p>
        
        <p>
          I am currently working on a project called ReviewBoard (<span style="color: rgb(6.670000%, 33.300000%, 80.000000%);">https://www.reviewboard.org/</span>). In short, it is a web based collaborative code review tool. I am not going to get into much detail about the project itself since you can find out everything from their homepage. The mentors for this project have been fantastic so far and to be quite honest, I cannot ask for any better. All our mentors have been helpful and always willing to lend a hand whenever possible; I am very fortunate to be working on a project with such great folks. We have our team meetings on IRC and in the chat, there are usually a couple of mentors ready to answer any questions we may have. Some prefer audio/video conferences but I have found that it has worked extremely well for us to just use IRC to do most of our communication. It allows other mentors and students to chime in on an issue or just discuss anything in general; it saves all the pain of trying to schedule a meeting with everyone that is involved in a discussion. I started on ReviewBoard doing simple bug fixes just to get familiar with the code base and working with Django. I have never worked with Django but once you get started on bugs and projects, everything will start to fall into place. Be sure to ask questions when you are stuck! I, for one, like to figure things out
        </p>
      </div>
    </div>
  </div>
</div>

<div class="page" title="Page 2">
  <div class="section">
    <div class="layoutArea">
      <div class="column">
        <p>
          by Googling so I sometimes spend hours figuring out the problem and realizing at the end that it was an easy fix. Sometimes when you are really stuck, dig around for yourself first then ask questions once you have given up searching. I think most people in UCOSP will agree: it is best to work in chunks than to give an hour of your time here and there. It may be tough to find a chunk of time but if you try both and compare the two approaches, you will find that you are much more productive working with chunks of time.
        </p>
        
        <p>
          For those interested, I will dive a bit deeper into ReviewBoard so you get a better glimpse of what goes on behind the scenes and what I have learned so far in regards to the technical side of things. As mentioned earlier, ReviewBoard is a free collaborative web based code review tool. It is currently being used by many big players in the industry such as Cisco, VMware, Twitter, LinkedIn, Amazon and many more. As you can probably tell, ReviewBoard can work with companies and organizations of any size. For me, ReviewBoard was not too difficult to get a grasp of; the code base is very clean and organized so locating pieces of code is easy once you get the hang of it, they are where you will expect them to be. The ReviewBoard code base also consists of Djblets and RBTools. Djblets (pronounced jiblets) are a set of useful extensions that ReviewBoard uses, this includes a datagrid, logging utilities, site configuration tools and much more. On the other hand, RBTools is a set of client tools that allow the user to perform tasks in the command line without accessing the interface. All three code bases are very well organized and documented, so it makes things easier if you are trying to figure things out on your own.
        </p>
        
        <p>
          My first easy fix bug was an issue with the user/group autocomplete functionality where it would be too ‘aggressive’. More specifically, the autocomplete functionality was selecting the first item that matched and once the user typed any more text, it would still autocomplete to the first item that it matched. Python was very familiar to me but not Django so I had to spend some time at the beginning to get used to the code I was reading. I found that the Django documentation on their homepage (https://docs.djangoproject.com/en/1.7) were helpful in getting started and understanding how Django works as a whole. If you are more of a visual oriented person then YouTube has plenty of good videos that explain more or less the same thing the documentation covers. Your browser’s developer tools are also a great tool to have under your belt. Without knowing where anything in the code base is located, you can use the developer tools to find out some key information (id, class, etc.) of what you are trying to modify then using that to perform a search on your code base can lead you to the right spots in the code to modify. There will be a lot of “aha!” moments once you see how everything is organized. Once the bug isfixed we check it into our local repository managed by git and post it up for review using RBTools. I realized that I did not know git fully when I had worked with it in a distributed project like ReviewBoard. It starts to bring out the all the things I thought I knew, but really did not, if that makes sense. It truly is a one of a kind learning experience that you cannot obtain from your typical Computer Science course.
        </p>
        
        <p>
          The first project I started to work on for ReviewBoard was allowing users to download all file attachments associated with a review request. First thing I did was brainstorm what I had to do, plan out each step and where the code should be placed. I like to make empty functions as
        </p>
      </div>
    </div>
  </div>
</div>

<div class="page" title="Page 3">
  <div class="section">
    <div class="layoutArea">
      <div class="column">
        <p>
          placeholders so it will help me visualize how the entire feature will work in code. The way Django works is by having a URL dispatcher that determines which view to be called depending on which URL it matched. A view in Django takes a user request and returns a response, usually the response is filling in a template with the appropriate information. This feature did not need a template since all it needed to do was send back a zip file of all the file attachments. The feature was relatively straightforward to implement except handling files from external sources. ReviewBoard allows the administrator to set up where user uploaded file attachments are stored, it can be locally on the server, on an Amazon S3 instance or an OpenStack Swift instance. I knew a lot of the code would be similar so I tried to make sure I coulddo it as easily as possible without duplicating code. It turns out that I could leverage file-like objects (StringIO package) to read local and external files into an object and then write it out to the resulting zip file. After some extensive testing, and a few peer reviews, it should be ready to ship!
        </p>
        
        <p>
          Next up for my student project, I will be working on adding functionality for the command line tools (RBTools), to enable the tools to search for the matching review request for a given commit. This is helpful when a developer makes new commits to their repository and needs to update the review request, they no longer have to manually input the review request ID and instead the tool can automatically find it for them. The function already exists for some RBTool functions so I will reuse the existing code to implement it for other functions that are missing this feature.
        </p>
        
        <p>
          So that is it! This is my UCOSP experience so far and I hope you learn a thing or two from my experiences. I am definitely looking forward to the rest of the term but sad at the same time that it will be over shortly 🙁
        </p>
        
        <p>
          TL;DR enroll in UCOSP and ask questions!
        </p>
        
        <p>
          If you have any questions, please feel free to ask!<br /> The UCOSP steering committee are a great bunch, so don’t be shy!
        </p>
      </div>
    </div>
  </div>
</div>