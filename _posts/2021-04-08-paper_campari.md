---
title: CAMPARI Camera-Aware Decomposed Generative Neural Radiance Fields
date: 2021-04-08
permalink: /posts/2021/04/08/paper_campari/
categories:
- paper-reading
tags:
  - arxiv
  - 3D reconstruction
  - neural rendering
---

learn a camera generator with image generator
- scene model: camera around a foreground object, with a background never collide with camera
  - shape / appearance code for foreground and background model -> conditioned nerf
- supervision from discriminator
- camera model: 5 params: fx fy, radius, elevation, azimuth
  - camera = camera_prior + offset