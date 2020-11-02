---
title: View Extrapolation of Human Body from a Single Image
date: 2020-02-24
categories:
- paper-reading
permalink: /posts/2020/02/24/paper_view_extrapolation/
tags:
- CVPR
- novel view synthesis
- image synthesis
---

task: single image human body synthesizing
- combine a shape estimation and image generation network
- human body, unlike other regid models, varies much due to deformation
    - thus gen. flow besed on depth map is much needed: rgb image -> depth map -> forward flow(using camera metrix) -> backward flow -> new image
- loss: image loss and flow loss: L1
