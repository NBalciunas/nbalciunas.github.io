---
author: Nojus Balčiūnas
pubDatetime: 2024-10-02T00:00:00
title: Red boat, Grey boat
slug: red-boat-grey-boat
featured: true
tags:
  - projects
  - "2024"
description: RC controlled boats I worked on during my summer job
---

| Year |  Status   |
| :--: | :-------: |
| 2024 | Completed |

## Boats, boats, boats

This summer I got hired to work on some RC controlled boats.
The grey boat is part of an Erasmus+ project of several countries with the goal of teaching students and children about making and controlling such boats.
I was hired to work on its electronics. The boat itself was made by some other very skilled people.
The red boat is meant to be a food delivery drone on water.
I worked on it during an internship before and a bit during summer.

## Grey boats electronics

I needed to make the whole thing be controllable with some controller and to make it collect a lot of data with a lot of sensors.
I used an Arduino Due for the boat and an Arduino Uno for the controller.
The boat and the controller were communicating with NRF24.
When the sensors, I needed to add pH, distilled oxygen, temperature, GPS, accelerometer sensors and some others.
All the info from sensors needed to be saved to a SD card and some info needed to be sent back to the remote like battery voltage and connection strength.
All this was done in a span of about 2 months.

## Red boats electronics

Working on the red boat was hard since a lot of people have worked on it before.
It was a real challenge trying to find ways to fix its problems not knowing where to start.
It was being controlled by a Pixhawk 6C and working with Pixhawk was also a challenge.
In the end I did not finish my work with this boat since summer was coming to an end.
I did manage to make fix some quirks here and there though.

## The Pictures

![](../../assets/images/red-boat-grey-boat/1.jpg)
![](../../assets/images/red-boat-grey-boat/2.jpg)
![](../../assets/images/red-boat-grey-boat/3.jpg)
![](../../assets/images/red-boat-grey-boat/4.jpg)
![](../../assets/images/red-boat-grey-boat/5.jpg)
![](../../assets/images/red-boat-grey-boat/6.jpg)
![](../../assets/images/red-boat-grey-boat/7.jpg)
![](../../assets/images/red-boat-grey-boat/8.jpg)
![](../../assets/images/red-boat-grey-boat/9.jpg)
![](../../assets/images/red-boat-grey-boat/10.jpg)
![](../../assets/images/red-boat-grey-boat/11.jpg)
![](../../assets/images/red-boat-grey-boat/12.jpg)
![](../../assets/images/red-boat-grey-boat/13.jpg)
![](../../assets/images/red-boat-grey-boat/14.jpg)
![](../../assets/images/red-boat-grey-boat/15.jpg)
![](../../assets/images/red-boat-grey-boat/16.jpg)
![](../../assets/images/red-boat-grey-boat/17.jpg)
![](../../assets/images/red-boat-grey-boat/18.jpg)
![](../../assets/images/red-boat-grey-boat/19.jpg)
![](../../assets/images/red-boat-grey-boat/20.jpg)
![](../../assets/images/red-boat-grey-boat/21.jpg)
![](../../assets/images/red-boat-grey-boat/22.jpg)
![](../../assets/images/red-boat-grey-boat/23.jpg)
![](../../assets/images/red-boat-grey-boat/24.jpg)
![](../../assets/images/red-boat-grey-boat/25.jpg)
![](../../assets/images/red-boat-grey-boat/26.jpg)
![](../../assets/images/red-boat-grey-boat/27.jpg)
![](../../assets/images/red-boat-grey-boat/28.jpg)
![](../../assets/images/red-boat-grey-boat/29.jpg)
![](../../assets/images/red-boat-grey-boat/30.jpg)
![](../../assets/images/red-boat-grey-boat/31.jpg)
![](../../assets/images/red-boat-grey-boat/32.jpg)
![](../../assets/images/red-boat-grey-boat/33.jpg)
![](../../assets/images/red-boat-grey-boat/34.jpg)
![](../../assets/images/red-boat-grey-boat/35.jpg)
![](../../assets/images/red-boat-grey-boat/36.jpg)
![](../../assets/images/red-boat-grey-boat/37.jpg)
![](../../assets/images/red-boat-grey-boat/38.jpg)
![](../../assets/images/red-boat-grey-boat/39.jpg)
![](../../assets/images/red-boat-grey-boat/40.jpg)
![](../../assets/images/red-boat-grey-boat/41.jpg)

<center>
<video width="600" height="auto" controls>
  <source src="/assets/red-boat-grey-boat/1.mp4" type="video/mp4">
</video>
</center>
<center>
<video width="600" height="auto" controls>
  <source src="/assets/red-boat-grey-boat/2.mp4" type="video/mp4">
</video>
</center>
<center>
<video width="600" height="auto" controls>
  <source src="/assets/red-boat-grey-boat/3.mp4" type="video/mp4">
</video>
</center>
<center>
<video width="600" height="auto" controls>
  <source src="/assets/red-boat-grey-boat/4.mp4" type="video/mp4">
</video>
</center>
