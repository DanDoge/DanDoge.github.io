---
title: Im2Avatar Colorful 3D Reconstruction from a Single Image
date: 2019-10-18
categories:
- paper-reading
permalink: /posts/2019/10/18/paper_im2avatar/
tags:
- 3D reconstruction
- texture synthesis
---


data representation
- jointly representing color and shape?
- separate representation

new loss
- false positive cross-entropy on unoccupied adn occupied voxels
- 3D to 2D flow, loss defined on flow
    - sample for occlusion parts and rough regions
    - balance the regressed color and sampled color
