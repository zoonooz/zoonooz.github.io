---
layout: post
title:  "📱Android Beam NFC NDEF Push to Reader"
date:   2012-06-21 20:29:07
categories: portfolio
thumbnail: /img/preview/nfc.png
platform: android
image: /img/portfolio/nfc.jpg
social: ['<iframe src="https://ghbtns.com/github-btn.html?user=zoonooz&repo=Android-Beam-NFC-NDEF-Push-to-Reader&type=watch&count=true" height="20" width="90" frameborder="0" scrolling="0" style="width:90px; height: 20px; margin-bottom: -6px" allowTransparency="true"></iframe>']
---

Receive simple NDEF messages (SNEP) pushed from Android ICS in P2P mode via the "Touch to Beam" feature to an ACS ACR122U reader.

![image](/img/portfolio/nfc.jpg)
{: style="text-align: center"}

  * It can only receive simple text NDEF messages (more than 255 bytes)
  * Uses Initiator mode to manually set LLCP connection parameters

<br/>

##### Tested on

  * ACS ACR122U firmware 207
  * Nexus S with Android ICS 4.0.3

<br/>
<br/>

Thanks to nfcip-java [https://code.google.com/p/nfcip-java/](https://code.google.com/p/nfcip-java/)
