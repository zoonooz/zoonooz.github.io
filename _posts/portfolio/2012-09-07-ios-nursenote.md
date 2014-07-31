---
layout: post
title:  "Nurse Note iPad Application"
date:   2012-09-07 20:29:07
categories: portfolio
thumbnail: /img/preview/nursenote.png
platform: ios
image: /img/portfolio/nursenote.jpg
---

When I was working at Kluaynamthai Hospital, I build one iPad application call **Nurse Note**. The main purpose of this app is for the nurses to record the data of patients.

<center>
![image](/img/portfolio/nursenote1.jpg)
</center>

The app working by fetch list of patients from the WCF service provided by another team, record data and send back to the server. I used [wsdl2objc](https://code.google.com/p/wsdl2objc/) to generate classes for connect with the service. 

<center>
![image](/img/portfolio/nursenote2.jpg)
</center>

Another requirement for this app is the data can save in offline mode when there is no internet and send that data back when it comes online.

<center>
![image](/img/portfolio/nursenote3.jpg)
</center>