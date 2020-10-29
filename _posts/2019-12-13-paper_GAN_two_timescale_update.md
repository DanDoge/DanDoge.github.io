---
title: GANs Trained by a Two Time-Scale Update Rule Converge to a Local Nash Equilibrium
date: 2019-12-13
categories:
- paper-reading
tags:
- GAN
- NIPS
---

under the condition that critic learns faster than the actor
- separate learning rates
    - a(n) = o(b(n))
- the distriminator must learn new patterns before transfor to generator
- Adam: escape local minima that leads to mode collapse
- introducing FID: consistent with increasing disturbances and human judgement
