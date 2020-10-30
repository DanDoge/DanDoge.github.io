---
title: View Independent Generative Adversarial Network for Novel View Synthesis
date: 2019-08-26
categories:
- paper-reading
permalink: /posts/2019/08/26/paper_vigan/
tags:
- GAN
- novel view synthesis
---

## View Independent Generative Adversarial Network for Novel View Synthesis

encoder-decoder architecture
- encoder: view-independent feature
- decoder: feature with user specific viewpoints
- ...and more
    - discriminators: classify real/gen images; pose estimation of input image
- ability to gen views outside the training set
    - 3d structure in latent space
- input: img[:3] + camera_pose[:12], camera pose provided for each pixel...
- coord conv instead of standard conv: concate pixel location
- and adain regularizer... fancy
- and yet tons of regularizer...gg
    - how are these back propagated? need src code
- encoder help 3d learning
    - feature from encoder feed into other 3d tasks
