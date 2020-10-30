---
title: PROGRESSIVE GROWING OF GANS FOR IMPROVED QUALITY, STABILITY, AND VARIATION
date: 2019-12-12
categories:
- paper-reading
permalink: /posts/2019/12/12/paper_progressive_gan/
tags:
- ICLR
- GAN
---

generative models
- autoregressive models: sharp images but slow, no latent representations
- VAE: easy to train but blurry results
- GAN: shapr but limited variations
    - gradients points to random directions when fake & real image not overlapping
    - higher res. makes discrimination easier
    - unhealthy competition when signal magnitute escalate in G and D

PROGRESSIVE GAN
- coarse to fine: (smoothly) add single layer once at a time
- learning an easy task at one stage
- batch std: each feature at (x, y), avg, concat
- normalize layer by c(from He. et al.), normalize feature vector after each layer
- similarity to Laplacian pyramid
