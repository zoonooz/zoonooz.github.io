---
layout: post
title:  "🦙Himabu"
date:   2016-01-18 00:00:00
categories: portfolio
platform: android
---

My first application here in Japan is [Himabu](https://www.himabu.com) for Android. I was working as an Android developer at [Nanameue](https://nanameue.jp/) to create this application which already exists in the iOS Appstore.

**Himabu** is the social application that focuses on students. We want them use their free times to communicate, make new friends and have fun with other students around Japan. Students can create a group, chat, call or post something to public timeline.

![image](/img/portfolio/himabu.png)
{: style="text-align: center;"}

At first, The app was built entirely using **Java** and then I decided to rewrite everything to **Kotlin** after half year released as the language becomes more stable. The code is easier to read and because I am using RxJava everywhere, the lambda expression from Kotlin helps shorten code a lot.

This app also supports conference call both voice and video. I created the **WebRTC** wrapper library from Google's libjingle that handle signaling and ICE for both iOS and Android app and integrated it as well.

[![Download Here](/img/download/playstore.png)](https://play.google.com/store/apps/details?id=com.shuapps.himabu)
{: style="text-align: center"}
