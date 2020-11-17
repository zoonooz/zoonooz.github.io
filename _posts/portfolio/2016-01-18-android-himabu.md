---
layout: post
title:  "🎓ひま部"
date:   2016-01-18 00:00:00
categories: portfolio
platform: android
---

>Himabu was shutdown and replaced by [Yay!](https://note.com/yay_official/n/n94e9e7b9f038) on 1th January 2020.

My first application here in Japan is Himabu for Android. I was working as an Android developer at [Nanameue](https://nanameue.jp/) to create this application which already exists in the iOS Appstore.

**Himabu** is the social application that focuses on students. We want them to use their free times to communicate, make new friends and have fun with other students around Japan. Students can create groups, chat, call or post something to public timeline.

![image](/img/portfolio/himabu.png)
{: style="text-align: center;"}

At first, The app was built entirely using **Java** and then I decided to rewrite everything to **Kotlin** after half year of its release as the language becomes more and more stable. The code is easier to read and because I am using RxJava everywhere, the lambda expression from Kotlin helps shorten the code a lot.

This app also supports conference call both voice and video. I created the **WebRTC** wrapper library from Google's libjingle that handle signaling and ICE for both iOS and Android app and integrated it as well.