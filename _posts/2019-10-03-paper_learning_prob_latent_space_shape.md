---
title: Learning a Probabilistic Latent Space of Object Shapes via 3D Generative-Adversarial Modeling
date: 2019-10-03
categories:
- paper-reading
permalink: /posts/2019/10/03/paper_learning_prob_latent_space_shape/
tags:
- 3D generation
- NIPS
---


what makes a good generative model for 3D models?
- varied and specific: fine details
- beyond memorizing and recombining

our model
- distangled representations for generative and discriminative models
- 200D latent vector
- all-conv nn
- discriminator learns faster than generator
    - 3D latent space hard to learn
    - discriminator updated only if acc. <= 80%

"distangle": by experiment, not by design
