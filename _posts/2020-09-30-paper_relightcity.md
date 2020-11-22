---
title: Learning to Factorize and Relight a City
date: 2020-09-30
permalink: /posts/2020/09/30/paper_relightcity/
categories:
- paper-reading
tags:
  - ECCV
  - reflection modeling
  - image synthesis
---

scene -> temporally-varying and permanent factors
- by encoding into higher-level latent factors
- intrinsic image equation: I = RS
- images -> illumination descriptor + sun angle -> shading images * average reflectance -> reconstruction
  - rotate geometry factor by sun angle
  - sunlight and skylight, per-pixel mixing weight