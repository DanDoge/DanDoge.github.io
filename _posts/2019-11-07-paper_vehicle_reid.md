---
title: list of paper on vehicle reid
date: 2019-11-07
categories:
- paper-reading
tags:
- vehicle reidentification
---

## list of paper on vehicle reid

- Group-Sensitive Triplet Embedding for Vehicle Reidentification
    - diverse but limited data -> modeling of appearance variance of each car
    - large scale of cars
    - training objective: min intra-class dist. s.t. inter-class dist. > threshold
    - triplet loss: class center & group center
- Vehicle Re-identification by Fusing Multiple Deep Neural Networks
    - siamese on Alex, VGG, FRCNN feature map
- Deep Relative Distance Learning: Tell the Difference Between Similar Vehicles
    - same as the first paper
    - diff. fc head for attribute recog. & embedding
        - special marks for identification
- Unsupervised Vehicle Re-Identification using Triplet Networks
    - detector and tracker -> feature extractor -> matching
    - require video data
- Viewpoint-aware Attentive Multi-view Inference for Vehicle Re-identification
    - 5 views for a car: front, side, rear, and two in the middle
    - input image -> feature -attention-> 5 map of diff. area masks -> discriminator v.s. real images
        - how realistic is generated masks?
        - attention? central point feature in each vp cluster
- Learning Coarse-to-Fine Structured Feature Embedding for Vehicle Re-Identification
    - fine-tune using images from the same vehicle
