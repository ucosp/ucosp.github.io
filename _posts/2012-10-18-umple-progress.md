---
id: 2902
title: UMPLE Progress
date: 2012-10-18T21:46:33+00:00
author: rtholmes
layout: post
guid: http://ucosp.ca/?p=2902
permalink: /winter-2012/2012/10/umple-progress/
categories:
  - Winter 2012
---
Stuart Erskine checks in from the UMPLE team.

Umple is a powerful tool for Model-Oriented Programming. It allows the
  
programmer to work on a more abstract level by generating code automatically for attributes, associations and state machines. This eliminates the writing of a lot of \_boiler plate code\_ when developing and speed up the development process. We are so confident in Umple&#8217;s code generating capabilities that \*we even write Umple using Umple\* 🙂

The Umple team consists of 6 members this term. They have made a few
  
decesions on how best to improve the process.

\*Thomas Morrison\* has accepted the challenge of allowing special ordering of association elements. Currently association elements are added in the order they are created and it would be useful to have other ordering methods. (Issue 184) \*Stuart Erskine\* is now working on allowing associations to interfaces. At minimum we should be able to have a one directional association, but ideally classes that implement interfaces should generate the required methods and thus allow for bi-directional associations.

\*Andrew Paugh\* has accepted issue 231 and is working on generating more meaningful comments. Because umple has the ability to mix in parts of a class from many different umple files, finding the source from generated code would be difficult. This commentary would allow future users to debug code much easier so they could find the origonal umple file from generated code much easier.

\*Russell Staughton\* has expressed intrest on two possible issues. One is working more on the Papyrus generation. Another is dealing with compositions and aggregation. When you delete an object you sometimes want to delete all the objects an item contains.

\*Sacha Bagasan\* is currently working on issue 318, the detection of proper state machine syntax. Currently when umple does not understand code found in an umplefile it outputs it as other code assuming it is means to be compiled in the target language. This may lead to confusion when it was meant to be umple code and a warning message was not presented to the user.

\*Christopher Hogan\* has accepted the task of adding constraints on the before and after capability. The idea is we want to be able to limit what possible values a class attribute may have, or likewise, what kinds of associations the class is allowed to have.