---
title: Learning-Based View Synthesis for Light Field Cameras
date: 2020-10-14
permalink: /posts/2020/10/14/paper_lbvs/
categories:
- paper-reading
tags:
  - SIGGRAPH
  - novel view synthesis
---

estimate disparity of novel view from features from input views
- warp input images(pay attention to direction when the word "warp" is used)
  - warp all input views to predefined disparity levels
  - then pass through a color CNN
- extreme few input images, low viewpoint variance