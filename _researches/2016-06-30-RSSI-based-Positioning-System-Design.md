---
title: "RSSI based Positioning System Design"
collection: researches
permalink: /research/2016-06-30-RSSI-based-Positioning-System-Design
excerpt: 'Quadrilateral diagonal intersection positioning algorithm with the distance weighted preprocessing is proposed to reduce the positional error by 20%.'
datestart: 2015-05-01
dateend: 2016-06-30
venue: 'School of Electronic Engineering, UESTC'
program: 'UESTC Innovation and Enterprise Program'
mentor: Engr. Bo Chen
location: Chengdu, China
---

Background
===
Received Signal Strength Indicator (RSSI) positioning method is one of the common modern communication positioning techniques. The method takes the phenomenon of the signal strength attenuation with the increase in distance to discover the position of an anchor. The positional error exists due to the several disturbance in the propagation of the electromagnetic wave, which results in the differences between the calculated distance through the attenuation coefficient and the practical distance.

System Design Scheme
===
* Cosidering the existing [triangle centroid positioning algorithm](/images/rsrch-2016-06-30-1.png) making use of _three intersections_ to figure out the position of one anchor, we managed to involve four to add more information and put forward the corresponding [quadrilateral diagonal intersection positioning algorithm](/images/rsrch-2016-06-30-2.png).
* Applied the distance of each intersection as the weighted coefficient to increase the effect of nearer intersection on the final calculation.
![distance weighted prepocessing](/images/rsrch-2016-06-30-3.png)
* Simulated the whole design on the Matlab platform.

