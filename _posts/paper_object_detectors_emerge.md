---
title: OBJECT DETECTORS EMERGE IN DEEP SCENE CNNS
date: 2019-08-09
categories:
- paper-reading
tags:
- object detection
- ICLR
---

## OBJECT DETECTORS EMERGE IN DEEP SCENE CNNS

CNN works well on diff. datasets and tasks, but what does it learn?
- this paper: CNN learns object detector in an  **unsupervised** manner when trained on scene understanding tasks.
- simplifying images: at each iteration, remove a segment which produces the smallest decrease in classification score
    - key objects remained
- **empirical** reception fields: smaller(~1/2) than theoretical size
- compared to CNN trained on Imagenet, CNN trained on scene understanding focus more on object in high level layers
    - object detector as internal representation of scene understanding?
- AP: ranging to >90%!
