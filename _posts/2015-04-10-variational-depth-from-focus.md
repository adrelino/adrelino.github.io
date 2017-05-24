---
layout: post
title: "Variational Depth from Focus Reconstruction"
---

I'm happy that our [variational-depth-from-focus](variational-depth-from-focus) project that we developed during the [Practical Course: GPU Programming in Computer Vision](http://vision.in.tum.de/teaching/ss2014/gpucourse_ss2014), is finally online. It is a CUDA implementation of ["Variational Depth from Focus Reconstruction"](https://arxiv.org/pdf/1408.0173v2.pdf) [Moeller 2015].

### Intro
The whole idea is that you can get a depth map from a set of aligned, differently focused images. This technique can be used e.g. in movie productions to capture the static 3d geometry of a scene to add special effects later on or in microscopy to get an elevation map of the probe.

### Abstract
>This paper deals with the problem of reconstructing a depth map from a sequence of differently focused images, also known as depth from focus or shape from focus. We propose to state the depth from focus problem as a variational problem including a smooth but nonconvex data fidelity term, and a convex nonsmooth regularization, which makes the method robust to noise and leads to more realistic depth maps. Additionally, we propose to solve the nonconvex minimization problem with a linearized alternating directions method of multipliers (ADMM), allowing to minimize the energy very efficiently. A numerical comparison to classical methods on simulated as well as on real data is presented.

### Example
We recorded this sequence of 19 differently focused images http://in.tum.de/~haarbach/balcony.zip (19 images, 8.7MB)  
The first image of the sequence is shown below:
![balcony_in](http://home.in.tum.de/~haarbach/balcony_0002.jpg)
After running our algorithm, we get the following smooth depth map:
![balcony](https://raw.githubusercontent.com/adrelino/variational-depth-from-focus/master/samples/results/balcony.png)




