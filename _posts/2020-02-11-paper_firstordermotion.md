---
title: First Order Motion Model for Image Animation
date: 2020-02-11
categories:
- paper-reading
permalink: /posts/2020/02/11/paper_first_ordermotion/
tags:
- NIPS
- image synthesis
---

decouple apperance and motion information by a self-supervised formulation
- a set of learned keypoints and local affine transformations
    - thus called "first order" method
- an occlusion-aware generator: infer background pixels from the context which is not included in source image
- trained by reconstruct a training video
    - predict a dense motion field
    - approx. transformations from sets of sparse trajectories (didnot get it...)
- losses
    - reconstruction loss based on perceptual loss
        - and on diff. number of resolutions
