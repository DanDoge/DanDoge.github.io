---
title: Photo-geometric autoencoding to learn 3D objects from unlabelled images
date: 2019-10-20
categories:
- paper-reading
permalink: /posts/2019/10/20/paper_photo_geometric_AE_learning/
tags:
- 3D reconstruction
---


learn from unlabelled data
- minimal assumptions
- previous works: with priors, monocular learning is possible
    - what prior?
- learn from unconstrained images
    - diff. views of diff. identities
- insights
    - var. in images gen.ed by vp. geometry and texture
    - registeration of vp. reduces var. significantly
- network
    - image -> vp / depth map / light / albedo -> rendered image --> loss
- gonna re-read later...confused
