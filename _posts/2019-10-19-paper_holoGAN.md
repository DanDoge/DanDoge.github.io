---
title: HoloGAN Unsupervised Learning of 3D Representations From Natural Images
date: 2019-10-19
categories:
- paper-reading
permalink: /posts/2019/10/19/paper_holoGAN/
tags:
- image synthesis
- GAN
- ICCV
---


unsupervised learning of 3D representations from 2D images
- view-dependent mapping from 3D to 2D
- generator: perturb pose of obj in input image
    - z as style vector
    - transformation & proj.: insight from camera system
- loss
    - identity of latent var.
    - style discriminator
- gonna refer to code for more details
    - well, quite intrinsic
