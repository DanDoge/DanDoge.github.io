---
title: Learning Disentangled Joint Continuous and Discrete Representations
date: 2019-12-21
categories:
- paper-reading
permalink: /posts/2019/12/21/paper_disentangled_continuous_discrete/
tags:
- NIPS
- disentangle learning
- VAE
---

goal: disentanglement on continuous and discrete variables
- revisit beta-VAE: larger beta leads to efficient and disentangled representations
    - KL as a upper bound of mutual information
    - penalizing KL improves disentanglement at the cost of reconstruction error
    - controlled information capacity -> force KL to be C, which increases during training
- approx. of discrete variables
    - Gumbel: differentiable relaxation
- diff. C for continuous and discrete variables
    - avoid model assigning all capacity to continuous var.s
