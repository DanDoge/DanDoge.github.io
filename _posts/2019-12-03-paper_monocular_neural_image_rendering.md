---
title: Monocular Neural Image Based Rendering with Continuous View Control
date: 2019-12-03
categories:
- paper-reading
permalink: /posts/2019/12/03/paper_monocular_neural_image_rendering/
tags:
- CVPR
- novel view synthesis
- neural rendering
---

task: real-time monocular novel view synthesis
- w/ continuous viewpoint control
    - previous work overfit to training settings
- input image -> latent code -> transformed latent code -> depth map -> bilinear sampling from input image -> output
- unable to gen. image w/ large viewpoint discrepancy?
- L_1 distance... not useful in my setting at all
