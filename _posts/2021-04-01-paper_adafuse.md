---
title: AdaFuse Adaptive Multiview Fusion for Accurate Human Pose Estimation in the Wild
date: 2021-04-01
permalink: /posts/2021/04/01/paper_adafuse/
categories:
- paper-reading
tags:
  - arxiv
  - pose estimation
---

enhance feature in occuluded viers by leveraging feature in visible views
- point-line corrspondence: point in one view correspond to a line in another view
  - aggragate multiple lines, find a optimal estimation from sampson distance
  - heatmap fusion
- adaptive weight for fusion
  - from appearance: some conv, mlp
  - from geometry: get sampson distance -> mlp
  - shared weight learning network