---
title: Beyond Face Rotation Global and Local Perception GAN for Photorealistic and Identity Preserving Frontal View Synthesis
date: 2019-09-09
categories:
- paper-reading
permalink: /posts/2019/09/09/paper_beyond_face_rotation/
tags:
- novel view synthesis
- ICCV
---


deal with pose variations
- hand-crafted features: find local distortion, metric learning
- deep-learning methods: tradeoff btw. invarience and discriminability
    - blurry and loss of details
- ill-defined prob.(good point here from optimization's point of view)
    - failure to provide with prior and constraints lead to blurred images
    - we use GAN as constrains
        - GAN outputs a grid of 0/1: focus on specific region

two-path
- local path for key part

loss
- pixelwise loss
- symmetry loss
- perceptual loss as identity preserving constrains
