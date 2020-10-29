---
title: Automatic Unpaired Shape Deformation Transfer
date: 2020-02-11
categories:
- paper-reading
tags:
- SIGGRAPH
- 3D reconstruction
---

learn how shapes deform from a dataset, provide a differentiable metric measuring visual similarity, mapping between latent space
- a VAE for source and target dataset
    - CycleGAN on latent code from two VAEs
    - two discriminator
- shape representation from previous papers
    - conv on mesh
- similarity measurement: learned by a NN
- training: seperately
