---
title: IBRNet Learning Multi-View Image-Based Rendering
date: 2021-02-26
permalink: /posts/2021/02/26/paper_ibrnet/
categories:
- paper-reading
tags:
  - arxiv
  - neural rendering
---

learn a view interpolation function **generalize** to other scenes
- more applicable than NeRF
- aggregate 2D feature from source views -> density feature
- ray transformer: transformer on density value
- ray marching -> proj points to neighbor views
  - feature pass though a MLP -> pooled to get a density -> sa on a  ray
  - feature with relative view direction -> weight for color (that is for a single point)