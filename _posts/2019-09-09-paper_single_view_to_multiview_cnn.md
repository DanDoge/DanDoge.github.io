---
title: Single-view to Multi-view Reconstructing Unseen Views with a Convolutional Network
date: 2019-09-09
categories:
- paper-reading
permalink: /posts/2019/09/09/paper_single_view_to_multiview_cnn/
tags:
- novel view synthesis
- ECCV
---

## Single-view to Multi-view Reconstructing Unseen Views with a Convolutional Network

encoder-decoder network
- trained on randered Shapenet models
    - generlizes well on natual images
        - well...semantically labelled natural images
- predict depthmap besides color images
    - 3D information... visualized by t-SNE on hidden embeddings

lit. review
- image transformation
    - DBM, gated autoencoder: do not scale to large images
    - transforming autoencoder: do predefined transformation
    - multi-view perceptron:
    - interpolate between similar models
- 3D model from single image
    - keypoint annotation
    - images from simalar models
    - need explicit 3D model

model
- input image ==> CCCCCL, desired vp ==> LLL
- concat, LLLCCCCC

drawback
- fail to capture finer details
    - high varience in distribution of details in dataset

another importance of best view selection?
- provide the most informative view for novel view synthesis
- and for 3D reconstruction
