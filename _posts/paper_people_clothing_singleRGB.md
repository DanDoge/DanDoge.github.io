---
title: Learning to Reconstruct People in Clothing from a Single RGB Camera
date: 2019-10-30
categories:
- paper-reading
tags:
- texture synthesis
- 3D reconstruction
- CVPR
---

## Learning to Reconstruct People in Clothing from a Single RGB Camera

input data & model
- people rotating in frnt of a singla camera
- semantic segmentation and 2D keypoint detection
- avg. pool on multiview data

related work
- well, not quite easy to understand for me

predefined shape model: SMPL
- and keypoint connectivity? confused

loss
- vertex L_2 loss
    - not EMD or chanfer: predefined topology
- vertex loss in posed space
    - supervises pose and shape
- silhouette overlap
- vertex SMPL loss: ?
- loss on pose params
- loss on joints?
