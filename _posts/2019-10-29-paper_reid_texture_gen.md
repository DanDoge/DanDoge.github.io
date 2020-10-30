---
title: Re-Identification Supervised Texture Generation
date: 2019-10-29
categories:
- paper-reading
permalink: /posts/2019/10/29/paper_reid_texture_gen/
tags:
- texture synthesis
- CVPR
---

## Re-Identification Supervised Texture Generation

Re-Id based texture synthesis
- perceptual loss restricts quality of textures
    - and L_1 results in blurred images
    - specified model to design loss!
        - need to find a car re-id model now...
- SMPL body model
    - estimate human pose
    - then deform the predefined model
- keypoint loss: face, hand
