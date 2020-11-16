---
title: Neural Reflectance Fields for Appearance Acquisition
date: 2020-09-28
permalink: /posts/2020/09/28/paper_reflectancefield/
categories:
- paper-reading
tags:
  - arxiv
  - neural implicit fields
  - reflection modeling
---

data aquisition
- phone with a builtin flash

light along camera ray and reflected from light source
- single light source in this setting
- pre-compute sampled points
- mlp outputs rgb, normal and other params for the reflection model
  - microfacet model, karris' approximation
  - also can use other models, like those for fur
- COLMAP for camera param. crop center regions to avoid background pixels