---
title: Neural Articulated Radiance Field
date: 2021-04-14
permalink: /posts/2021/04/14/paper_narf/
categories:
- paper-reading
tags:
  - arxiv
  - 3D reconstruction
  - neural rendering
---

human as a tree of joints
- a point in space can belong to different joints -> different coordinate systems
  - feed all possible coordinates under all joints to a single nerf
    - weighted by a small MLP(selector)