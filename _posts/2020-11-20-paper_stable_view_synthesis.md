---
title: Stable View Synthesis
date: 2020-11-20
permalink: /posts/2020/11/20/paper_stable_view_synthesis/
categories:
- paper-reading
tags:
  - arxiv
  - neural rendering
  - novel view synthesis
---

geometric scaffold from SfM and MVS
- on-surface feature aggregation: directional feature vector processed to produce a new vector
- SfM and MVS: colmap
- for each point, query the set of images where the point is visible
- encoder: imagenet pretrained resnet18, batchonrm frozen
- fc graph of features and a graph attention network 
- a sqeuence of unet for rendering
