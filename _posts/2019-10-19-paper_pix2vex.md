---
title: Pix2Vex Image-to-Geometry Reconstruction using a Smooth Differentiable Renderer
date: 2019-10-19
categories:
- paper-reading
permalink: /posts/2019/10/19/paper_pix2vex/
tags:
- 3D reconstruction
- texture synthesis
---


threefold contributions
- C^{infty} smooth differentiable renderer
- image2geometry NN: predict 3D coordintes of given topology
    - due to its diff. nature, DR's output is diff. from real world images
    - introduce a new module to map to real image field
- reconstructive adversial network
    - to discriminate the mapping module mentioned above

renderer
- view transformation: triangles -> proj. coor.
- resterization: triangles -> pixels
    - keep a z-buffer
    - ...of prob. of visible triangles
    - softmin-based function: differentiable!

reconstructor
- pre-defined topology
- conv-deconv-fc-sigmoid
