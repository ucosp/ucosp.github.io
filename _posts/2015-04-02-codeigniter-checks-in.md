---
id: 2977
title: CodeIgniter checks in
date: 2015-04-02T13:18:35+00:00
author: rtholmes
layout: post
guid: http://ucosp.ca/?p=2977
permalink: /winter-2015/2015/04/codeigniter-checks-in/
categories:
  - Winter 2015
---
<p class="p1">
  <span class="s1">Xing Zeng from UToronto who has been working on the CodeIgniter project checks in on this term.</span>
</p>

I am working on the CodeIgniter Project. More specifically, our team is spending most of our time in developing Netbeans plugin for CodeIgniter developers.

CodeIgniter is a light-weight PHP framework, loosely based on the popular Model-View-Controller development pattern. It is the 4th most widely-used PHP framework throughout the Internet[1]. Despite this, there has been no IDE plugin for it on any major IDE, where lots of other PHP frameworks, including the famous Symphony and the not so famous Nette2, all have IDE plugins specifically designed to work with the features of their library. That&#8217;s the reason why our team decided to work on it.

The first platform we choose to implement our plugin was Netbeans. It is a fast and flexible IDE and it is among the preferred choice of many CodeIgniter developers as well as the IDE being taught in the CodeIgniter class at BCIT. It has tons of libraries and APIs for you to develop plugins conveniently to work with Netbeans. Since Netbeans was programmed in Java, our Plugin is also written in Java, created in Netbeans IDE as a Netbeans Module Project. Some other supplementary files were written in PHP.

This is the first time I have ever worked on an open source project as well as the first time I ever started working on an open source project from the ground up. We use Github as our major tool for issue tracking and source control, just like a lot of other open source libraries including CodeIgniter itself. So I really feel excited about this golden opportunity, and I do feel I learn something from it. The following are two examples of what I have learned from participating in this project.

The first target I set was to implement a view navigation functionality. It is a fairly easy task since Netbeans has already provided you the interface _HyperlinkProviderExt_ for you to implement. So I approach this naively at first, directly go into the package of code navigation to do all my coding work. I did kind of realize that this is not the correct way at the beginning of implementing a somehow complicated software, as some of my functionality in parsing Hyperlink and retrieving files may also be required by other parts of the program. But I did not have a chance to think about it carefully until I have decided how am I supposed to integrate the interface in _HyperlinkProviderExt_ with the functionality I want. This turn out to be a problem later, when one of my team members came to me and ask me how to tokenize the PHP file, which is a functionality I have implemented after I finished my code. The result of not having a consensus prior to working on the code is a minor refactoring required in my code to make the system work and a major one is still ongoing for both my package and the shared package to make the code more clear and robust.

Then I switched to working on the auto-completion functionality. For this part, I realized that learning from other open source projects on Netbeans IDE Plugin is extremely useful, which is also a major reason why people promote open source. This is even more essential in my case since, for some reason I don’t know, Netbeans APIs does not have javadoc with it and it takes so much time to manually go over its online documentation. So, I looked into some other open source projects, including the source code for the Yii Plugin, wojciech-holisz plugin, as well as the Sprint Autocompletion file and the structure of the Zend Plugin. They gave me lots of help on providing me a basic idea of how the structure of my _CompletionProvider_ class could be and showing me what kind of API calls as well as pre-defined object would be convenient for me to use. This allowed me to finish the coding of this part early and understand how each part could  work together.

In conclusion, I feel like working for CodeIgniter is a really great opportunity and I do feel I learned a lot from it.

**
  
[1] http://www.sitepoint.com/best-php-frameworks-2014/**