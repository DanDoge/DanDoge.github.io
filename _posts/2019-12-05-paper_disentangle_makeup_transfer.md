---
title: Disentangled Makeup Transfer with Generative Adversarial Network
date: 2019-12-05
categories:
- paper-reading
permalink: /posts/2019/12/05/paper_disentangle_makeup_transfer/
tags:
- CVPR
- disentangle learning
---

task: disentangle identity and makeup
- an encoder for each task
    - assumption: identity and makeup independent of each other
    - perceptual loss for personal identity preservation
    - histogram matching on diff. regions, then L_2 loss for makeup transfer
- attention mask for each key part
    - face, brow, eye, lip
