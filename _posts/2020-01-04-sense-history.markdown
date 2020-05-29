---
layout: post
title: sense-history 
date: 2020-01-12 13:32:20 +0300
description: Explore your city from a different perspective. How often do you cross the former Berlin Wall on your way to work? How many trees older than 100 years do you pass? 
img: berlin_wall.png # Add image post (optional)
fig-caption: Source: OpenStreetMap# Add figcaption (optional)
tags: [Raspberry Pi, Technology & Society, Maps]
---



Have you ever wondered how often you would have to cross the former Berlin Wall on your daily route to work? Which trees were already there 100 years ago? Where did during the Second World War people find shelter from military attacks? 

We all have the tools to answer these questions. However, it can be challenging to relate to these numbers and to put them into perspective. What does it actually mean to split a city right in the middle with a 140 kilometer long wall?

The goal of *sense-history* is to make parts of a cities' history perceptible.

It is a wearable device that signals historic landmarks. So, while going through your daily life you can get a sense on how your city looked years ago, discover the history of its buildings and experience the dimension of historic changes.
As soon as you are near a historic landmark or if you cross the Berlin wall *sense-history* will vibrate.

Raspberry Pi Setup | Wrist band with vibration module 
:-------------------------:|:-------------------------:
 ![]({{site.baseurl}}/assets/img/full_setup.jpg) | ![]({{site.baseurl}}/assets/img/wearable.jpg) 


### Modules

In general, any geospatial data can be transformed into a module.
A module takes care that the geospatial data is interpreted correctly and squared with the current GPS location. 

Right now, It's possible to signal a vibration in two different use cases:


	(1) when the current location is close enough to a point of interest in the data
  e.g. when we are standing in a 2 meter radius of a tree older than 100 years

	(2) when a specific line is crossed or predetermined areas are entered or left
  e.g. when crossing the Berlin wall from east to the west sector (or the other way around)


At the moment four modules are available:

- The Berlin Wall
- Historic Points in Berlin
- Trees in Berlin
- Trees in Zurich



Finding adequate geospatial data can be time-consuming and tedious. If you have ideas for modules, tips for sources or even processed data, please create a pull request or reach out to me.



The full code can be accessed on [GitHub](https://github.com/Tilana/sense-history).

It also contains documentation about

- [the hardware setup](https://github.com/Tilana/sense-history/blob/master/docs/HardwareSetup.md)
- general background information on [satellite navigation and geographical coordinates](https://github.com/Tilana/sense-history/blob/master/docs/GPS.md)

