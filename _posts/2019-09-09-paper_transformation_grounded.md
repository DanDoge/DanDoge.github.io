---
title: Transformation-Grounded Image Generation Network for Novel 3D View Synthesis
date: 2019-09-09
categories:
- paper-reading
permalink: /posts/2019/09/09/paper_transformation_grounded/
tags:
- novel view synthesis
- CVPR
---


infer visible parts, then complete image
- difficult task: pixel occlusion
- more explicit access to 3D information
    - first predict transformation of pixels & visibility map
        - vis_map * flow(input)
        - visibility aware, zero-out background
    - condition generation
        - bottle-neck forwarded with information from DOAFN
        - refines distortion
        - hallucinates missing parts
    - loss network
        - euclidean distance between feature of real and gen. images
        - VGG16: color consistancy, but blurry
        - adv.: sharp but has artifacts
- experiment on synthetic and real images
    - synthetic data + rando backgrounds for real images

lit. review
- geometry based
    - reconstruct 3D scene then synthesize novel views
    - interpolate between neithboring views
    - fail to deal with discclusion
    - data-driven: limited by existing models
- image generation networks
    - encoder-decoder network: blurry and low res. from disentangling factors from single-view, and smooth measures(L1 or L2)
    - deep network as loss function: perceptual loss
    - GAN introduced
    - image completion
