---
layout: post
title:  "Playing with Estimote Beacon"
date:   2014-07-30 20:29:07
categories: blog
tag: [swift]
---

I just got a new project from my boss which is using [Estimote](http://estimote.com/). I cannot write about the purpose of this app but I will write about what it is and how I use it.

## What is Estimote Beacon ?
- - -

>An Estimote Beacon is a small, wireless device, sometimes also called a 'mote'. When placed in a physical space, it broadcasts tiny radio signals to smart devices.  --- from estimote website

So basically it is a small device that broadcasts a radio signal. But what is that signal and how it works?

Estimote Beacon broadcasts signal using [Bluetooth LE](http://en.wikipedia.org/wiki/Bluetooth_low_energy) and [iBeacon](https://developer.apple.com/ibeacon/) standard which is implement Bluetooth's Proximity sension specification. You can think of it as a someone that keep shouting **"Hey, I am here. My name is ..."** every second.

Estimote Beacon broadcasts signal with the following data:

```
Proximity UUID: B9407F30-F5F8-466E-AFF9-25556B57FE6D
Major: 1234
Minor: 5678
```
**Proximity UDID** : Unique identifier of the beacon. As default, the value will be the same for all device that comes from Estimote but you can change it later.

**Major** : Most significant value of beacon. You can use it as group number.

**Minor** : Least significant value of beacon. You can use it as member number in group.

## Development
- - -

The main concept of this app is just notify the user when the phone is close to any of Estimote devices and the notification must include the information that can indicate which device user is close to. For example 

## Conclusion