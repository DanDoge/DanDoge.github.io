---
title: ALIGNFLOW LEARNING FROM MULTIPLE DOMAINS VIA NORMALIZING FLOWS
date: 2019-12-05
categories:
- paper-reading
tags:
- ICLR
- image synthesis
---

objective: learn a joint distribution over two domains
- CycleGAN
    - indirect constraint of joint distribution
    - careful design of loss functions
- a single latent variable shared by two domains
    - forward mapping implemented as a normalizing flow: cycle consistant in nature
    - also can be trained by MLE objective
        - only trained by MLE fails to identify optimal mapping: any volume-preserving transformation in latent space will achieve the same L_{MLE}
