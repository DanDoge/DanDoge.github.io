---
title: Visual Object Networks Image Generation with Disentangled 3D Representation
date: 2019-10-03
categories:
- paper-reading
permalink: /posts/2019/10/03/paper_visual_object_network/
tags:
- image synthesis
- NIPS
---


shape code -> voxel grid -> depth map + silhouette map -> 2D image
- first step: vanilla gan
- second step: viewpoint estimation from real data
- last step: cyclegan-ish
    - one-to-many mapping: latent code ignored in one-to-one assumption
    - add one loss: E_text(G_text(v_2.5d, z_text)) ~= z_text
    - and L_KL to let E_text close to a Gaussian
