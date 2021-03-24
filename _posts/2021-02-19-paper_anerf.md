---
title: ANeRF Surface-free Human 3D Pose Refinement via Neural Rendering
date: 2021-02-19
permalink: /posts/2021/02/19/paper_anerf/
categories:
- paper-reading
tags:
  - arxiv
  - neural rendering
  - pose estimation
---

test-time optimization
- monocular motion capture
- SPIN for pose estimation
  - SMPL human model
- joint-relative encoding: point to nearest joint(well, actually assign a weight for this), render under this coordinate
- large batchsize -> stable training