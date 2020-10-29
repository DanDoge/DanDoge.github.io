---
title: VQA Visual Question Answering
date: 2019-08-22
categories:
- paper-reading
tags:
- VQA
- ICCV
---

## VQA Visual Question Answering

what is "AI-complete"?
- require multi-modal knowledge, beyond a single domain
- well-defined quantitative evaluation metric

provide a dataset
- images from MSCOCO
- 3 questions per image
    - open end, free form
    - low-level and commonsense level
    - are images necessary / too strong commonsense?

- network
    - image -> hidden layer
    - question -> lstm / bow
    - then concat these layers, fc
