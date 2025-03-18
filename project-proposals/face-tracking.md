---
title: "Face Tracking"
date: 2021-07-01T00:00:00-04:00
draft: false
---

## Problem Statement

This is a typicl vsual computing task. The goal is to improve the performance of the face tracking algorithm (see the video below). The algorithm is implemented in Python using OpenCV. Current version exploits thresholding *segmentation* and *tracking* based on simple features like energy and velocity vrector.


<video width="640" height="480" controls>
  <source src="../videos/track.mp4" type="video/mp4">
  Your browser does not support the video tag.
</video>

## Suggestions

One may consider other types of segmentation like edge-based segmentation. As for tracking, one may try a simple *SORT* usung Kalman filter. 

## More ambitious ideas
>Super resolution and face normalization

In ideal case, we would like to normalize faces. However this is a very challenging task due to a very low resolution of the video. We would need faces to be at least 60 x 90 pixels. To increase the resolution, we may consider using a super-resolution algorithm. 
