---
title: Discovery of Latent 3D Keypoints via End-to-end Geometric Reasoning
date: 2020-02-01
categories:
- paper-reading
permalink: /posts/2020/02/01/paper_keypointnet/
tags:
- NIPS
- 3D keypoints
---

task: given a single image, to extract 3D keypoints **optimized for downstream tasks**
- network: image ->  ordered list of 3D points: pixel coordinates and depth values
    - N heads for N keypoints
- downstream task: relative pose estimation
    - multiview conssitency loss: discrepancy between two set of points
    - relative pose estimation loss: distence of two rotation matrix under F norm
- output a distribution map: spatial softmax layer
- symmetry: predict whether the object is facing left or right
    - location of [1, 0, 0] and [-1, 0, 0]
- separation loss
    - avoid degeneration
- silhouette loss
    - only allowing non-zero prob. inside the silhouette
- and penalize the variance of distribution map
    - helps in case of non-convex object boundaries
