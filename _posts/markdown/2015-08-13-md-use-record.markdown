---
layout: post
title:  "markdown使用记录"
date:   2015-08-14 11:23:32
categories: markdown
tags: markdown jekyll
---

## **自定义post时间格式**  
***  
打开_layouts\\post.html  
将\{\{ page.date \| date: "%b %-d, %Y" \}\}修改为\{\{ page.date \| date: "%Y年%m月%-d日" \}\}

## **修改post的摘要**  
***  
截取post的前一段内容用作摘要:  
\{\{ post.content \| strip_html \| strip_newlines \| truncate: 160 \| remove: '<p>' \| remove: '</p>' \}\}  
