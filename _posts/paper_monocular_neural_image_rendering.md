---
title: Monocular Neural Image Based Rendering with Continuous View Control
date: 2019-12-03
categories:
- paper-reading
tags:
- CVPR
- novel view synthesis
---

task: real-time monocular novel view synthesis
- w/ continuous viewpoint control
    - previous work overfit to training settings
- input image -> latent code -> transformed latent code -> depth map -> bilinear sampling from input image -> output
- unable to gen. image w/ large viewpoint discrepancy?
- L_1 distance... not useful in my setting at all
