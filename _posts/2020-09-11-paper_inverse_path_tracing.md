---
title: Inverse Path Tracing for Joint Material and Lighting Estimation
date: 2020-09-11
permalink: /posts/2020/09/11/paper_inverse_path_tracing/
categories:
- paper-reading
tags:
  - CVPR
  - neural rendering
  - reflection modeling
---

differentiable MC renderer, inverse path tracing
- geometry is most given, material and lighting are missing
- path tracing is computationally expensive and non-convex and ill-posed
  - variance reduction and other regularization 
  - L1 norm good: robust to outliers
- each **object** has a single emission and meterial parameters