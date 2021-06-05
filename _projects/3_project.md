---
layout: post
title: Work Zone Detection
description: Color-based method for identifying work zone objects
---

According to the statistics provided by Federal Highway Administration, crashes occurred in work zones resulted in over 39000 injuries and 842 fatalities. Therefore, a work zone detection algorithm is an essential step in developing safety-focused driver assistance systems.

As a part of the Video Analytics project at Virginia Tech Transportation Institute, I developed a simple work zone object detector based on a Bayesian classifier. We used prior information about object pixel-wise color and spatial location on a 2D frame. This approach can be used as a preliminary data filtering step for a more robust deep learning classifier. You can find the example of a work zone image and classification results before and after post-processing below:

![workzone](/gradfolio/assets/images/workzone.jpg)

*Tools used: Python, OpenCV, Seaborn*