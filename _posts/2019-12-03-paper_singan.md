---
title: SinGAN Learning a Generative Model from a Single Natural Image
date: 2019-12-03
categories:
- paper-reading
permalink: /posts/2019/12/03/paper_singan/
tags:
- ICCV
- image synthesis
- GAN
---

task: unconditional image synthesis from a single image
- purely generative: noise to image
- hierarchy of patchGANS
    - coarse to fine: each stage inject random noise
    - training procedure: from coarse to fine stage, fixed former GANs after it's trained
    - WGAN-GP increases training stability
