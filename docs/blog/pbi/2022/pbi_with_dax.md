---
template: blog_comment.html
title: Develop custom date range slicer in Power BI
description: As a Power BI developer, there are chances that your user one day will request
    for a custom date range, other than the pre-defined date period selections. This post takes you to achieve that with ease.
date: 2022-01-17
hide:
  - navigation
  # - toc
tags: 
  - pbi
---

Supercharge your #powerbi report with #dax 



Just a few days ago while doing the final functional review with a client on a #powerbi project, the client requested for something funny but sincerely it really makes a lot of  sense :

 "custom date slicer with default date to  Today" i.e. By default when the user sign in to view the report, it will be filter to the current date and the same slicer can be used to change to any custom date range. 

<p hidden>#more</p>

My colleague said "that should be easy to do sir" but immediately  I replied this is the toughest request will have received on this project.



After further research, my colleague came back very sad that no such functionality exist in #powerbi  by default. Without this functionality the client will refused to sign off the project.



Fortunately after few hours of meditation , I came with the solution using #dax code and some report filtering functionality in #powerbi.



The Lesson: Learn to supercharge your #powerbi with #dax , you are only using 40% of #powerbi functionality without #dax. #dax has helped me to solved most of the request will received from client.

![img](https://media-exp1.licdn.com/dms/image/C4D22AQFqyyOezRhbkw/feedshare-shrink_800/0/1643441162639?e=2147483647&v=beta&t=-GjmnH7eGjS7NDQp0Z6MWO4OYn6FPnHreDLHz1GU9fA)

![img](https://media-exp1.licdn.com/dms/image/C4D22AQFQ5XUT2tlQhg/feedshare-shrink_800/0/1643441162676?e=2147483647&v=beta&t=YM7-IcCF_8n3QQLO7NApyn7vCSBfoQLIrrpN8H9-4aY)