---
title: Revisiting Unreasonable Effectiveness of Data in Deep Learning Era
date: 2019-09-05
categories:
- paper-reading
permalink: /posts/2019/09/05/paper_revisit_data_in_DLera/
tags:
- learning theory
- ICCV
---

## Revisiting Unreasonable Effectiveness of Data in Deep Learning Era

Paper reading could be a leisure after days of failed experiments

size of dataset remains the same while num of params and GPU power grows
- what if we have much more data?
- provide a *internal* dataset: JFT, 300m images
    - noisy annotations, 20% error after cleansing
- representation learning benefits!
- perofrance increases logarithmically based on size of training data
- model capacity influences gain on more data

representation learning
- using web-supervision or unsupervised method
    - deep clasifiers from images tags in the wild
        - from tags added by users
        - not that large a gap from annotations in Imagenet
        - Imagenet or Imagenot: short of images for some tags
        - problem: synonyms, misspelling and split-up tags
        - ...and tags far away from GT

50 GPUs...fine
- training for 2 months...
