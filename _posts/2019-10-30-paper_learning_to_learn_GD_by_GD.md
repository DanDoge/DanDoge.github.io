---
title: Learning to learn by gradient descent by gradient descent
date: 2019-10-30
categories:
- paper-reading
permalink: /posts/2019/10/30/paper_learning_to_learn_GD_by_GD/
tags:
- learning theory
- NIPS
---


hand designed optimization to learned ones?
- no free lunch: optimize in a specified field
- rethinking generalization

optimizer and optimizee
- L(phi) = E_f[f(theta(f, phi))]
    - a good phi should max. theta's performance w.r.t. target function f
    - sample f to update phi
- refer to code
