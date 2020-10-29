---
title: StarGAN Unified Generative Adversarial Networks for Multi-Domain Image-to-Image Translation
date: 2020-03-12
categories:
- paper-reading
tags:
- CVPR
- image synthesis
- GAN
---

scalable i2i translation on more than two domains
- single generator learns mapping between all domains
    - inputs image and domain information
- model
    - discriminator
        - GAN loss, domain classification loss
            - WGAN with gp, patchGAN
    - generator
        - GAN loss, reconstruction loss
- label construction
    - c = [c_1, ..., c_n, m], m being mask, eg. [00101 00000 10]
