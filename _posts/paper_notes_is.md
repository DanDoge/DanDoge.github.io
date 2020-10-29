---
title: A Note on the Inception Score
date: 2019-12-12
categories:
- paper-reading
tags:
- ICML
- image synthesis
---

goal: find a generative distribution s.t. p_G(x) ~ p_R(x) according to some metric
- an explicit p_G not availble
- findings
    - common metrics do not correlate with each other
    - no clear evidence that any model is better
        - up to a hyperparameter search

IS
- qualities: image contains clear objects, high diversity of images from all classes in ImageNet
    - note: unbalanced class distribution in ImageNet
    - correlate well with human judgement of quality
- problems
    - suboptimalities: depends on implementation / sensitive to weight change
    - usage: models trained other than ImageNet yields misleading results
