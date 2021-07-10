---
layout: post
comments: true
excerpt_separator: <!--more-->
title: "Day Thirty One to Thirty Five!"
subheading: "Workin' my ass off..."
date: 2021-07-10 11:06
image: /assets/img/post_bg/engerland.jpg
categories: PDM pybites django heroku
tags: [PDM, Blog, pybites, django, heroku]
---
Where has he been I hear you ask, a whole week and no social media or blog posts??? Well yes apologies for this but I have been in the trenches battling to finsh an early alpha release of my app and hit my deadline to get it to heroku. <!--more-->And did you do it?? Of course I bloody did.  
  
The app finally went live this morning after staying up until 2am for the final push. Fixed the last couple of issues, applied a custom domain and hey presto, bob's your uncle, the site is live. But not without it's flaws. The last six weeks have given me a completely new appreciation for how much work is involved in deploying an app of any sort to the web. Documentation, YouTube, Tutorials all make it look so easy, but none of them ever address the errors you may hit, and you will hit them.  
  
Sitting up until 2am trying to figure out why heroku is throwing a 400 error or a Bad Request error when everything was working locally is not a pleasant way to spend an eveing. The site worked with Debug set to true, maybe we should try that and see if we can figure out what is going wrong??... Turns out that setting is in fact extemely helpful in diagnosing problems. A few quick fixes in the code later, a bit of

```bash
git push heroku main
heroku logs --tail
```

set DEBUG back to false 

```bash
heroku config:set DEBUG=False
```

and everything springs into life!

Relief, time off this weekend well earned!

I won't reveal the domain just yet as I want to demo to my fellow PDM'ers on this weeks code-clinic if Bob will allow me to.  
  
The site still needs plenty of polish and consistency to make me completely happy, but as Bob and Julian always say
> Remember the 80/20 rule!!

  One day I should find out what they mean 😂🤣

Anyway thats enough rambling for one week. I now need to focus my energy on Sundays Euros Final (and I don't mean Eurovision!!) I've only been waiting my entire life for England to reach the Final in any football competition, let's hope they don't dissapoint as I don't think I've got another 50 years left in me!!