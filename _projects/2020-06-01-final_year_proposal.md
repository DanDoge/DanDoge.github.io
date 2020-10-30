---
title: 'Best View Synthesis of 3D objects'
date: 2020-06-01
permalink: /projects/2020/06/01/best_view_synthesis_of_3d_objects/
---

We proposed a new novel view synthesis(NVS) model that given a single image input, our model can synthesize images of the same object from arbitrary viewpoints. We extend previous NVS methods by disentangling the learned latent space into content and style sub spaces, s.t. our methods can be used to synthesize texture from realworld images. Experiment results show our method outpreforms classical NVS methods both quantitatively and qualitatively.

### Method

The pipeline of our method is shown below.

![](/images/banner.png)

While previous novel view synthesis methods focu on extracting view-independent information from input images, the latent code obtained is in fact disentangled. We believe that by disentangle the latent code into content(represented by depth map) and style(high-dimentional vector) code, the network will be more robust and learn view independent features more efficiently.

We derived a new ELBO in our case, since there are two(not one) latent varibles to be conditioned on. $i$, $c$, $s$ stands for image, content, style respectively.

![](/images/ELBO.png)

As shown in the above equation, the whole pipeline is trained by minimizing reconstruction loss of both depth image and rgb image and KL loss in latent space. Details about training procedure can be found at [Chap. 3-2](https://github.com/DanDoge/FYP/blob/gpu_0201_without_pair/thesis/template/%E6%9C%AC%E7%A7%91%E8%AE%BA%E6%96%87_%E5%AF%BC%E5%B8%88%E8%AF%84%E9%98%85%E8%A1%A8_%E9%BB%84%E9%81%93%E5%90%89_1600017857.pdf) (in Chinese).

### Results

We show the rotation result and latent code swap result below, more details can be found at [Chap. 3-3](https://github.com/DanDoge/FYP/blob/gpu_0201_without_pair/thesis/template/%E6%9C%AC%E7%A7%91%E8%AE%BA%E6%96%87_%E5%AF%BC%E5%B8%88%E8%AF%84%E9%98%85%E8%A1%A8_%E9%BB%84%E9%81%93%E5%90%89_1600017857.pdf) (in Chinese).

![](/images/novel_view_thesis_rotate.png)

![](/images/appendix_syn_swap.png)

### Applications

Our model can be used to define the best view of 3D model from the intuition that the best view should contain the most texture to reconstruct other views. Also our novel view synthesis network can be used to synthesize 3D models' texture given a single RGB image(synthesized or from real-world).