---
layout: post
title:  "AisleOne iPad Application"
date:   2015-09-27 20:29:07
categories: portfolio
platform: ios
---

**AiselOne** is shopping application that simulates the aisle of supermarket. User can scroll left and right to browse the product and simply drag and drop the it to the cart if you want to buy or schedule to have it later.

<center>
![image](/img/portfolio/aisleone1.jpg)
![image](/img/portfolio/aisleone2.jpg)

<iframe width="560" height="315" src="https://www.youtube.com/embed/eH_gPLy5J3E" frameborder="0" allowfullscreen></iframe>

</center>

The most challenging things are to make the app smooth as much as possible and use least memory. To make it smooth, I pre-load all the images into the memory (500+ images). But by doing that, the app got a lot of memory warnings and eventually crash :(

No other way, I have to trade the frame rates with the memory by using `NSCache` to hold references to those images. Best case, the app will be smooth as before, but in worst case, it will lag a lot. I personally want to use background thread to load image from disk, render and fade in to the cell to make the scrollig smooth, but it will not look realistic!

I am woking with the team at Gomeeki to make this app better and more stable. The app is now in Australian store. You can check it out.

<center>
[![Download Here](/img/download/itunestore.png)](https://itunes.apple.com/us/app/aisleone-afd/id1038268561?mt=8)
</center>
