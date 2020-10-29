---
title: RETHINKING STYLE AND CONTENT DISENTANGLEMENT IN VARIATIONAL AUTOENCODERS
date: 2019-12-01
categories:
- paper-reading
tags:
- disentangle learning
- variational autoencoders
- ICLR
---

disentanglement creteria/definition
- label & style preserving, i.e. for fixed style & label, model outputs images of same style and label

label preservation
- rewrite objective -> posterior regularization
- p(y | x) -> p_D(y | x)
    - hence the style can only be encoded in z
    - but style preservation may not hold

style preservation
- as domain adaptation: unsupervised
- VAE does not enforce style preservation

...so why VAE consistently learn disentangled representations?
- a shared encoder **or** decoder is sufficient for disentanglement
