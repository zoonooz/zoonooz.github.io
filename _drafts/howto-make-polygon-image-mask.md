---
layout: post
title:  "How to make polygon image mask"
date:   2014-11-30 20:29:07
categories: blog
tag: [swift,ios]
---

We all as iOS developer must have used `cornerRadius` property in `CALayer` to make our `UIImageView` to be round or circle according to the design from designer. But what if the designer want someting more than that, polygon? star?, what should we do.

This blog will show you how to use `UIBezierPath` to make a dynamic polygon to be mask for `UIImageView` like this

<center>
<img width="300" src="/img/blog/polygon-imageview/avatar.png" />
</center>