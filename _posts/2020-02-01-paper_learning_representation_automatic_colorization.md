---
title: Learning Representations for Automatic Colorization
date: 2020-02-01
categories:
- paper-reading
permalink: /posts/2020/02/01/paper_learning_representation_automatic_colorization/
tags:
- ECCV
- image synthesis
---

image pass through VGG16
- concat features in all conv layers
- train a fc layer for hue and chroma *histograms*
- loss: bin the Lab axes by evenly spaced Gaussian quantiles
    - apply KL loss
- findings
    - networks trained by colorization generalize well to other tasks
