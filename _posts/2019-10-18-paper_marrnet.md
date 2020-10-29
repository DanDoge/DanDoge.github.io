---
title: MarrNet 3D Shape Reconstruction via 2.5D Sketches
date: 2019-10-18
categories:
- paper-reading
tags:
- 3D reconstruction
- NIPS
---

## MarrNet 3D Shape Reconstruction via 2.5D Sketches

pipeline
- realworld-RGB -> 2.5D sketches -> 3D shape
- both stage uses an encoder-decoder network
    - and a reprojection consistency loss: on depth map, siloette map, normal map
- train on synthetic images and fine-tune on real-images
    - synthesize image of random viewpoints
    - finetune with decoder fixed
