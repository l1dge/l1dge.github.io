---
layout: post
comments: true
excerpt_separator: <!--more-->
title: "Day Eighteen!"
subheading: "I'm losing my mind."
date: 2021-06-16 19:32
image: /assets/img/post_bg/post_bg005.jpg
categories: PDM pybites django error
tags: [PDM, Blog, pybites, django, error]
---
So its been a bit since my last post, six days to be exact if you include the weekend. To be honest its been a crappy few days trying to track down an elusive bug (still haven't found it!) and I had to walk away from the PC for a while or I was going to destroy something!!  
<!--more-->I had to refactor the authentication model again as I was getting some weird issues with user registration, this is now fixed at the command line in that I can now run a django command to create x number of users or superusers. However in doing this I have introduced the elusive bug which causes django to try and do a double insert violating a unique key. This only happens in the form and for the life of me I cannot understand why. I'm sure it has something to do with the form save and me extending the django user model. Good job I have a code clinic with Bob tomorrow.  
So whilst I have been a bit absent from social media and blogging I have not been sat on my laurels. I found an excellent django plugin called Djang-debug-toolbar, without which I would have lost my mind (still a possibility). Hopefully normal service will resume tomorrow and Bob will see how stupid I've been and just go straight to the issue (here's hoping!).  
If we can't find the bug I may reverse the user model changes and start again.  
  
So thats the latest, back again tomorrow if all goes well!