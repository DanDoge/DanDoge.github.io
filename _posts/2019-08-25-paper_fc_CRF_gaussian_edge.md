---
title: Efficient Inference in Fully Connected CRFs with Gaussian Edge Potentials
date: 2019-08-25
categories:
- paper-reading
permalink: /posts/2019/08/25/paper_fc_CRF_gaussian_edge/
tags:
- image segmentation
- conditional random field
- NIPS
---

## Efficient Inference in Fully Connected CRFs with Gaussian Edge Potentials

multiclass image segmentation
- common approach: MAP inference in a CRF
    - inability to model long-range connections
- fc crf: slow
    - contribution: efficient inference algorithm: O(N) approximation
    - downsample, convolution, then upsample
- refer to paper for more details

I need to learn signal processing now...
