---
title: What Do Single-view 3D Reconstruction Networks Learn?
date: 2019-09-15
categories:
- paper-reading
permalink: /posts/2019/09/15/paper_what_do_single_view_3d_reconstruction_learn/
tags:
- 3D reconstruction
- CVPR
---

## What Do Single-view 3D Reconstruction Networks Learn?


"*We show that encoder-decoder methods are statistically indistinguishable from these baselines, thus indicating that the current state of the art in single-view object reconstruction does not actually perform reconstruction but image classification*"
- all use a encode-decoder structure
- sometimes worse than image recognition

experiment
- 55 classes
- recognition baselines
    - clustering, mean shape
    - retrieval
    - oracal nearest neighbor
- from Kolmogorov-Smirnov test, we cannot reject decoder-based methods are statictically essentially recogintion baselines
