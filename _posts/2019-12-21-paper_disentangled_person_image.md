---
title: Disentangled Person Image Generation
date: 2019-12-21
categories:
- paper-reading
permalink: /posts/2019/12/21/paper_disentangled_person_image/
tags:
- CVPR
- image synthesis
---

multibranched network: foreground, background, pose
- more control over images
- two stage training
    - train a embedding space first
    - then a mapping from Gaussian to that space: adverserial training
- pose mask: refer to paper
- pose invariant features: 7 body ROI
