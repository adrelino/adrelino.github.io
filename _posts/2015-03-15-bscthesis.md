---
layout: post
title: "3D Object Reconstruction using Point Pair Features"
permalink: "bscthesis"
---
I finally finished my bachelor's thesis. Here is the [final thesis](http://adrian-haarbach.de/bscthesis_adrian.pdf) as well as the [final presentation slides](http://adrian-haarbach.de/bscthesis_adrian_slides.pdf). All the code I developed during my research is open source and is hosted in my github repository [ppf-reconstruction](https://github.com/adrelino/ppf-reconstruction)

###Abstract
3D Object Reconstruction using Point Pair Features
>This work aims at reconstructing 3D objects by robustly and accurately registering multiple
range images of an object from different viewpoints.
An initial alignment between any two overlapping scans is obtained via a voting scheme
which matches similar point pair features and thus constrains the relative 6DoF rigid body
motion between the poses of two viewpoints. This initial alignment is then refined using
pairwise point-to-plane ICP. The result of this step is a tree of relative pose constraints.
In a subsequent global optimization step, we build up a graph of absolute poses, our
vertices, from the tree of initial relative pose estimates by adding further edges. We add
edges for the k-nearest-neighbors of a vertex, taking the translational difference of the
corresponding poses as a distance measure. Constraints between two vertices are added
for each closest point correspondence in their respective point clouds. The global point-toplane
energy is then minimized iteratively using the nonlinear least-squares method called
Multiview Levenberg-Marquardt ICP.
This refined registration of all the scans used may now be integrated and their corresponding
point clouds fused and then meshed to obtain the final reconstructed 3D object
mesh.


