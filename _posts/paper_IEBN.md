---
title: Instance Enhancement Batch Normalization an Adaptive Regulator of Batch Noise
date: 2019-08-17
categories:
- paper-reading
tags:
- optimization
---

## Instance Enhancement Batch Normalization: an Adaptive Regulator of Batch Noise

this paper focus on two kind of noises
- estimation noise: diff. between mean/var/loss of this batch and the whole dataset
- batch noise: loss of one instance disterbed by the batch information

self-attention is an adaptive noise regulator to enhancing instance specificity
- proposes an attention based bn

test on cifar, imagenet
- comparable result
- better results on style transfer?
    - only one example shown
- anti attack
- activation func: high influnce
