---
title: Unsupervised Learning of Object Landmarks through Conditional Image Generation
date: 2019-12-24
categories:
- paper-reading
tags:
- NIPS
- disentangle learning
---

learn landmark by looking objects from diff. vp
- a mapping gamma(x, phi(x')) = x'
- phi(x') being a set of landmark detections
    - avoid identical mapping
- heatmap -> renormalised to prob. dist.
    - softmax then condensed to a point
- perceptual loss
    - pretrained by colorising grayscale images
