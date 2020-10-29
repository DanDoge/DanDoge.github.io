---
title: Recurrent Transformer Networks for Semantic Correspondence
date: 2020-02-22
categories:
- paper-reading
tags:
- image synthesis
- NIPS
- semantic correspondence
---

first paper I've read on semantic correspondence
- objective: a field from src img to tgt img
- previous approaches
    1. infer the field in feature extraction step, by min. a objective function
    2. feature extraction -> predict field in a end2end manner
- this paper
    - conbine these two
        - feature extraction -> predict a field -> modify the feature using the field -> ...
    - matching phase: similarity using cosine distance
    - loss: "classification", does that mean this transformation should be better than other ones?
