---
title: IMAGE GANS MEET DIFFERENTIABLE RENDERING FOR INVERSE GRAPHICS AND INTERPRETABLE 3D NEURAL RENDERING
date: 2020-11-02
permalink: /posts/2020/11/02/paper_imagegan_dr/
categories:
- paper-reading
tags:
  - arxiv
  - neural rendering
---

styleGAN as a generator, extract 3D params., DR for reconstruction
- goal: extract and disentangle 3D knowledge by generative models
- GAN as a neural renderer
- styleGAN: lower layers for viewpoint, while higher layers for shape, texture and background
  - fine tune with inverse graphic network fixed
  - disentangle bg and fg with seperated losses