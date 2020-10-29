---
title: Unsupervised shape transformer for image translation and cross-domain retrieval
date: 2019-12-30
categories:
- paper-reading
tags:
- arxiv
- image synthesis
---

challenge: input and output do not share same geometrical information
- unpaired data
- CycleGAN: content in input and output images are aligned
- keeping appearance information while transfer shape information
    - object-focused: object in context
    - content space and style space shared
    - above constraints not enough when output is multi-model -> weak adverserial learning
    - attention: literially mask on middle layer
    - AdaIn by style
    - fit-in module: copy-paste in latent space
- losses
    - symmetry loss: inherent prior of clothing and faces
