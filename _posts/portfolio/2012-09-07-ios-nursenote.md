---
layout: post
title:  "👩‍⚕️Nurse Note iPad Application"
date:   2012-09-07 20:29:07
categories: portfolio
thumbnail: /img/preview/nursenote.png
platform: ios
image: /img/portfolio/nursenote.jpg
---

When I was working at Kluaynamthai Hospital, I build one iPad application call **Nurse Note**. The main purpose of this app is for the nurses to record the data of patients.

![image](/img/portfolio/nursenote1.jpg)
{: style="text-align: center"}

The app is working by fetching list of patients from the WCF service provided by another team, record data and send back to the server. I used [wsdl2objc](https://code.google.com/p/wsdl2objc/) to generate classes for connect with the service.

![image](/img/portfolio/nursenote2.jpg)
{: style="text-align: center"}

Another requirement for this app is the data can be saved in offline mode when there is no internet connection and be able to send that data back when it the internet available.

![image](/img/portfolio/nursenote3.jpg)
{: style="text-align: center"}
