---
title: DO 2D GANS KNOW 3D SHAPE UNSUPERVISED 3D SHAPE RECONSTRUCTION FROM 2D IMAGE GANS
date: 2020-11-09
permalink: /posts/2020/11/09/paper_2d_gan_3d_shape/
categories:
- paper-reading
tags:
  - arxiv
  - GAN
---

mine geometry clues from **off-the shelf** GAN
- pretrained GAN contains rich 3D knowledges, thus can be used to recover 3D shape from 2D images
- convex shape initialization, render pseudo samples
- 3 steps
  - initialize depth, reconstruction
  - render under different light and view, refine using GAN, reconstruction
  - refine depth map with all networks being trainable