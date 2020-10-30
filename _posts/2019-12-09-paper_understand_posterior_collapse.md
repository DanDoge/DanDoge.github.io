---
title: Understanding Posterior Collapse in Generative Latent Variable Models
date: 2019-12-09
categories:
- paper-reading
permalink: /posts/2019/12/09/paper_understand_posterior_collapse/
tags:
- ICLR
- variational autoencoders
---

postetior collapse
- variational distribution matches the prior for some dimentions
- previous work: the KL term causes it
- this paper: spurious local maxima in training objective
    - study from linear VAE: marginal distribution encourages postetior collapse
        - rotation matrix accounts for weak identifiability in the model
    - variance of the observation model impacts the stability of local stationary points
        - large sigma tends towards a stable local maxima
        - ELBO does not introduce any additional spurious local maxima
