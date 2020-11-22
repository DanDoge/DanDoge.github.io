---
title: GeLaTO Generative Latent Textured Objects
date: 2020-09-29
permalink: /posts/2020/09/29/paper_gelato/
categories:
- paper-reading
tags:
  - ECCV
  - neural implicit representation
  - 3D reconstruction
---

reconstruction of thin structures
- using plane as a proxy 
- generative latent optimization framework
  - identity latent variable(to be optimized) -> w -> neural textures of patches -> transform to target pose -> composed image
  - adversarial lossses lead to worse results, no regularization loss