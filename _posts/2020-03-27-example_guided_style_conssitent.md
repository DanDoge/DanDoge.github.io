---
title: Example-Guided Style-Consistent Image Synthesis from Semantic Labeling
date: 2020-03-27
permalink: /posts/2020/03/27/example_guided_style_conssitent/
categories:
- paper-reading
tags:
  - CVPR
  - image synthesis
---

image synthesis from semantic label map and exemplary image
- directly using pix2pixHD will not keep style well
- multiscale discriminator, feaure matching loss
- style consistenct loss on pair of images
    - dataset constructed from video
- semantic consistency loss
    - from VGG feature map
    - weighted perceptual loss: weight=1 for content consistent images, weight=1/M for style consistent images
