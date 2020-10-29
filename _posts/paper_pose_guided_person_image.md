---
title: Pose Guided Person Image Generation
date: 2019-12-21
categories:
- paper-reading
tags:
- NIPS
- image synthesis
---

generate an image conditioning on reference image and a specified pose
- coarse to fine: blurry result by L1 loss refined via adverserial training
    - better and faster: easy task to learn
    - predict a difference map: speed up training
    - true/fake pair: input pose / real pose
        - avoid trival solution: output input image in stage 2, maybe?
    - leverage L1 and adverserial loss
        - the latter causes artifacts
