---
title: NeRF Representing Scenes as Neural Radiance Fields for View Synthesis
date: 2020-09-03
permalink: /posts/2020/09/03/paper_NeRF/
categories:
- paper-reading
tags:
  - ECCV
  - neural implicit field
  - neural rendering
---

a volumetric scece implicit function by MLP
- ray marching: coarse stage -> fine stage
- radiance depends on viewpoint
- add some prior to occupancy distribution?
- volume rendering -> read papers...
- positional encoding
  - interesting...
- supervision only from RGB
  - with implicit multiview consistency constraint
- what can be extracted from mlp weights?