---
layout: post
title:  "Himabu"
date:   2016-01-18 00:00:00
categories: portfolio
platform: android
---

My first application here, after moved to Japan is [Himabu](http://www.himabu.com) for Android. I am working as an Android developer at [Nanameue](http://nanameue.jp/) to create this application which already exists in the iOS Appstore.

**Himabu** is the social application that focuses on students. To use their free times to communicate and make new friends with other students around Japan. Students can create a group, chat, call or post something to public timeline.

![image](/img/portfolio/himabu.png)
{: style="text-align: center;"}

At first, The app was built entirely using **Java** and then I decided to change to **Kotlin** after half year released as the language becomes more stable. The code is easier to read and because of I am using RxJava everywhere, the lambda expression from Kotlin helps shorten code a lot.

This app also supports conference calling both voice and video. I implemented the **WebRTC** wrapper library from Google's libjingle that handle signaling and ICE for both iOS and Android app and integrate it as well.

[![Download Here](/img/download/playstore.png)](https://play.google.com/store/apps/details?id=com.shuapps.himabu)
{: style="text-align: center"}
