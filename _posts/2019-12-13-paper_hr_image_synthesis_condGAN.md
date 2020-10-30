---
title: High-Resolution Image Synthesis and Semantic Manipulation with Conditional GANs
date: 2019-12-13
categories:
- paper-reading
permalink: /posts/2019/12/13/paper_hr_image_synthesis_condGAN/
tags:
- CVPR
- image synthesis
---

address two problems
- difficulty of generating images of high resolution
- lack of details and realisim

method
- aim: diverse result given input label map
    - object-level semantic editing
- global generator and local enhancer
    - two scales often enough
- 3 discriminators for different scales
    - easier to train coarse to fine
    - feature matching in each layer of distriminator
- instance-level semantic label map -> object boundry
- instance-wise average pooling
    - how to implement?
