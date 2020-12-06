---
title: Adversarial Generation of Continuous Images
date: 2020-12-03
permalink: /posts/2020/12/03/paper_agci/
categories:
- paper-reading
tags:
  - arxiv
  - neural implicit representation
---

neural implicit representation and GAN
- using a hyper network
  - train a shared weight prior and a offset for each layer
- factorized multiplicative modulation
- weight of each frequency predicted by latent variable
- better latent space: keypoint estimation from latent code(disentanglement)
- multiscale: append position from different resolution
  - another way to progressively grow network