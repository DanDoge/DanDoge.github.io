---
title: Weakly-supervised Disentangling with Recurrent Transformations for 3D View Synthesis
date: 2019-10-18
categories:
- paper-reading
permalink: /posts/2019/10/18/paper_weekly_disentangling_view_synthesis/
tags:
- novel view synthesis
- NIPS
---


observation
- human take time proportional to rotated angles in matching images of the same object
- recurrent: rotate 15 degrees once in a step

model
- encoder-decoder
- hidden unit: identity unit + pose unit
    - controlled by action unit
    - mimic the underlying manifold step by step
    - identity unit being shared while pose unit keeps changing
- also predict mask
