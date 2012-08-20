---
layout: post
title: "Check Duplicate in MySQL"
date: 2011-06-21 00:00
comments: true
categories: [Database, Code]
---
Simple snippet:

``` sql SQL to check duplicate entry
SELECT `name`, COUNT(`name`) as cnt
FROM `members`
GROUP BY `name`
HAVING cnt > 1
ORDER by cnt;
```