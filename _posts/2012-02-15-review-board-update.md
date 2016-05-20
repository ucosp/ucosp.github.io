---
id: 2859
title: Review Board Update
date: 2012-02-15T12:40:28+00:00
author: rtholmes
layout: post
guid: http://ucosp.ca/?p=2859
permalink: /winter-2012/2012/02/review-board-update/
categories:
  - Winter 2012
---
Curtis Muller writes:

We all know Review Board is great for allowing a distributed team to effectively ensure only high quality, standards complaint code is integrated into the end product. But what else makes Review Board great?

From my experiences on the team I can safely say it gives new developers a leg up on the learning curve when starting. I was able to leverage Review Board to quickly learn exactly what I should, and should not be doing in my code. Through each new code review I was determined not to repeat the same mistakes that were made in my previous review. The intuitive review interface clearly communicates these mistakes back to the developer, allowing them to make the changes and learn from their mistakes.

Review Board also acts as an effective communication platform for any distributed team utilizing it, as it allows the entire team to see the progress of each component, and add their own input to how the end solution should look. This is very important, as communication is one of the toughest aspects when working with a team not based in one site.

I started off in the Code Sprint by getting my feet wet with a couple bugs and a small project. Due to the fact that I haven’t used Django recently, and that the Review Board code base itself is quite large and complex this meant I was in for quite a steep learning curve. I have now moved on to my second project, which itself comes in two parts. The code based part of the project is a rating extension which will allow users to leave anonymous feedback on the quality of the code reviews they receive, while also tracking their own aggregated results over a period of time. These results will allow users to reflect on their code reviewing habits, and make improvements if necessary. This project will be leveraging brand new scripts to simplify the extension building process, by templating out the base code required for an extension to exist in a Review Board instance.

The second half of this project will involve writing documentation to guide others using these scripts on how to take their extension stub and turn it into a functional and integrated part of their Review Board environment. A lot of developers get the idea that by adding this “one feature” to the project, it will vastly improve their experience using Review Board. This has many problems however, because if every one of these features are added they will start to bloat the code base, making Review Board run slower and harder to maintain. This also requires developer hours, which could be spent working on other features which would benefit more than just a handful of developers. Adding this “one feature” also runs the risk of alienating other developers with features or functionality they don’t need, want, or understand. The great thing about extensions is that they allow these developers requesting the feature to easily create and add the feature to their own instance of Review Board, without impacting everyone else’s experience.

It’s great to be able to work on such a far reaching project like Review Board, and know my improvements are being used all across the world. The project could not be nearly as successful without the big effort put in by each of the mentors. Their ability to offer prompt code reviews, technical guidance, and project ideas really makes working on Review Board a lot of fun. Due to their efforts, more time is spent in the learning or “eureka” phases of development than stuck in a frustrating roadblock.