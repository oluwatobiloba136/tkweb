---
template: blog_comment.html
title: SQL Server 3-way Logic
description: SQL Server uses 3- way logic. Every logical expression evaluates to TRUE, FALSE or UNKNOWN (null).
    Whenever an unknown value is used in an expression, it evaluates to unknown.
date: 2021-11-12
hide:
  - navigation
  # - toc
tags: 
  - T-SQL
---

SQL Server 3-way Logic



Presume that your customer detail form allow that customer to decide if he or she will fill her phoen number, meaning the phone number is optional.  What does it mean 
if the customer does not enter a phone number and the table ends up with NULL in the 
PhoneNumber column of the Customer table? Does it mean that the customer does not 
have a phone? That’s one possibility

<p hidden>#more</p>

More possibility might occur, the customer might have phone number but decide to ascond your request for her phone number. 
<br>
As a data analyst, you are given a list of phone number to find if the customer number match any of them. To your surprise, your ssearch will return ***no match*** because you are searching for unknown value.
<br>
Usually, comparing the data in a column to a value or comparing the values from 
two columns returns either TRUE or FALSE. If the expression in the WHERE clause evaluates 
to TRUE, then the row is returned. If the expression evaluates to FALSE, then the row is 
not returned. 
<br>
If a value in the expression contains NULL, then the expression is resolved 
to UNKNOWN. In some ways, the behavior is like FALSE. When an expression resolves to 
UNKNOWN, the row is not returned. The problems begin when using any operator except 
for equal to (=). The opposite of FALSE is TRUE, but the opposite of UNKNOWN is still 
UNKNOWN.

To test for a NULL, you will want to use the IS [NOT] NULL expression. 
Additionally, you may want to change a NULL to a value like an empty string (''). 
The function ISNULL will replace a NULL value with another value specified in the 
query.

![img](https://media-exp1.licdn.com/dms/image/C4D22AQGXYgfBvz8ldQ/feedshare-shrink_800/0/1637077110543?e=2147483647&v=beta&t=qsFYbzhVAeJwj_b55zMGB0Q46ofrw7_0Cixv09cYy9w)