---
title: 'Multi-view 3D Models from Single Images with a Convolutional Network'
date: 2019-08-12
categories:
- paper-reading
permalink: /posts/2019/08/12/paper_multiview_model_from_single_image/
tags:
- 3D reconstruction
- ECCV
---

## Multi-view 3D Models from Single Images with a Convolutional Network

model
- input: image and desired viewpoint
    - viewpoint: azimuth, elevation(cos and sin), distance from object center
- output: image under desired viewpoint and depth image
- architecture: simple encoder-decoder architecture
- dataset: random viewpoint and location rendered shapenet models on random background image
    - panda3d renderer?

what's learned in latent variables?
- t-SNE: shape and color
- interpolating latent variables
