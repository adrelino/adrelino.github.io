---
layout: post
title: "Variational Depth from Focus Reconstruction"
permalink: "variational-depth-from-focus"
---

I'm happy that our CUDA implementation of Moeller, Michael, et al. [Variational Depth from Focus Reconstruction](http://arxiv.org/pdf/1408.0173v2.pdf). arXiv preprint arXiv:1408.0173v2 (2014).
that we developed during the [Practical Course: GPU Programming in Computer Vision](http://vision.in.tum.de/teaching/ss2014/gpucourse_ss2014) is finally online.

###Abstract
>This paper deals with the problem of reconstructing a depth map from a sequence of differently focused images, also known as depth from focus or shape from focus. We propose to state the depth from focus problem as a variational problem including a smooth but nonconvex data fidelity term, and a convex nonsmooth regularization, which makes the method robust to noise and leads to more realistic depth maps. Additionally, we propose to solve the nonconvex minimization problem with a linearized alternating directions method of multipliers (ADMM), allowing to minimize the energy very efficiently. A numerical comparison to classical methods on simulated as well as on real data is presented.
