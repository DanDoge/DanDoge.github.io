---
title: Everybody Dance Now
date: 2020-03-12
categories:
- paper-reading
tags:
- ICCV
- video synthesis
---

do as I do motion transfer
- with pose as a intermediate representation
    - human pose detectors, pretrained
    - pose stick figure: plot keypoints, draw lines
        - normalize using heights nad ankle positions
- x_t conditioned on x_{t-1}
    - but what is x_0? mentioned nowhere
    - and where does the bg come from?
- faceGAN for high quality
