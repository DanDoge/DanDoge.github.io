---
title: Learning View Priors for Single-view 3D Reconstruction
date: 2019-10-16
categories:
- paper-reading
tags:
- 3D reconstruction
- CVPR
---

## Learning View Priors for Single-view 3D Reconstruction

tackle on single-view reconstruction
- ambiguity in possible shapes
- prior knowledge of category
    - a discriminator on input view and random view
- following the diff. renderer
- 3D representation
    - deform a cube
    - texture and shape both defined on cube
- loss
    - recons. loss: diff in multiview
    - view discrimination loss
    - internal pressure loss: loss points outside
