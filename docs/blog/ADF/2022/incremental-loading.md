---
template: blog_comment.html
title: A simple incremental loading ADF Architecture
description: Part of being a good data engineer is knowing when to use which load type. The decision to use an incremental or full load should be made on a case-by-case basis
date: 2022-03-18
hide:
  - navigation
  - toc
tags: 
  - ADF
  - Azure
---

An incremental load is the selective movement of data from one system to another. An incremental load pattern will attempt to identify the data that was created or modified since the last time the load process ran.

<p hidden>#more</p>

A good scenario is when an excel file need to be update with employees that have been paid each and every pay day.

As a smart #finance person are you going to fill a new file from scratch for every pay day with the updated information of every employee? No.

A better option to take the file from the last pay day, remove the terminated employees, add the new hires and then update any promotion with Incremental loading.

Using #azuredatafactory simplifies this process for flat files like #excel

![img](https://media-exp1.licdn.com/dms/image/C4D22AQG5KnLcPgwE9g/feedshare-shrink_800/0/1647318598387?e=2147483647&v=beta&t=QBk_F4KIHZyHK3MH_dzcNH8VaSsRf0419-Pcyxee7qU)