---
title: View Synthesis by Appearance Flow
date: 2019-09-11
categories:
- paper-reading
permalink: /posts/2019/09/11/paper_view_synthesis_appearance_flow/
tags:
- novel view synthesis
- ECCV
---

## View Synthesis by Appearance Flow

human has the ability to recover 3D model from 2D images
- Science 1971 paper...mental rotation
- app.: 3D photo editing, image-driven VR

past approaches
- geometry based: estimate 3D, transform pixels
    - i'd better read one paper on this
    - 3D structure hard to get
    - occlusion-caused wrong hole-filling
- learning based
    - parametric model for **one** class...as stated in paper, true?
    - blurry

our method
- gen. a apperance flow
    - no need to gen. pixel from scratch
    - preserving identity
    - bilinear interpolation
- and a foreground prediction
    - deal with blurriness...i guess
- for multiple view inputs  
    - predict a conf. map for each view
- alleviates blurriness
- color indentity perserved
- intuitive interpretation of the network

lit. review
- disentangling pose and identity
    - view manipulations restricted to small rotations
- CNN for view synthesis
    - apperance flow better than pixel gen.
- geometric view synthesis
    - rely on finding visual correspondence
    - fail to cope with multiview input
    - interpolate btw. nearest models
- texture synthesis
    - reuse input image
