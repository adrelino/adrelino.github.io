---
layout: post
title: "Continuous time trajectory estimation for 3D SLAM from an actuated 2D laser scanner"
permalink: "mscthesis"
---
I finally finished my master's thesis. Here is the [thesis](http://static.adrian-haarbach.de/mscthesis_adrian.pdf) as well as the [presentation](http://static.adrian-haarbach.de/mscthesis_adrian_slides).

### Abstract
This thesis aims at estimating trajectories for 3D SLAM applications. A continuous time
formulation allows solving multiple problems inherent to the traditional discrete time approaches
seamlessly, such as sensor fusion of actuated 2D laser scanner data with inertial
measurements. Special care is taken when choosing an appropriate trajectory representation.
The well-known ICP algorithm used for rigid registration is extended significantly so
it can deal with continuous-time, multi-view registration of deformable scans. The resulting
algorithm can be employed online in a time-windowed fashion to get an open-loop trajectory
estimate and offline for global optimization to further reduce the drift. In contrast
to previous work we are able to provide ground truth data for evaluation by extending
an existing simulator so that it can simulate actuated 2D laser scanner data with corresponding
inertial measurements. Experiments on synthetic data with different scenarios,
noise levels and parameter settings show the versatility, stability and adaptability of our
algorithm as well as its high overall accuracy.
