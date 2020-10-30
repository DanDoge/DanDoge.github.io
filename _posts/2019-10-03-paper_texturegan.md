---
title: TextureGAN Controlling Deep Image Synthesis with Texture Patches
date: 2019-10-03
categories:
- paper-reading
permalink: /posts/2019/10/03/paper_texturegan/
tags:
- image synthesis
- CVPR
---

## TextureGAN Controlling Deep Image Synthesis with Texture Patches

user guided image generation
- high res. details
- propagate texture to object boundaries
- wrap texture: infer 3D infromation

tons of losses
- pixel loss, style loss and content loss through VGG, Adversarial loss
    - GAN loss on gray images: deal with colorful texture
- introducing LAB color space
    - content and texture on L, color on AB
- what if no data of this specific object with this texture
    - def new loss only on given texture
