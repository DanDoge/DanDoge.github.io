---
title: Few-Shot Generalization for Single-Image 3D Reconstruction via Priors
date: 2019-10-26
categories:
- paper-reading
permalink: /posts/2019/10/26/paper_fewshot_recons_w_priors/
tags:
- 3D reconstruction
- few shot learning
- ICCV
---


category priors
- prior shape + input image
- sparsity of output space -> lack of data
    - need priors!
- generalize to novel object with no additional training
    - generatizability of NN rather than fewshot method
- so... quite similar to conditional U-Net
    - with iterative refinement
    - in multiview case: one new image in one step
