---
title: Pyroomacoustics
layout: project
tagline: "Fast image sources and array processing algorithms"
description: "A python package providing fast image source model for shoebox and polygonal rooms."
klass: software
permalink: /pyroomacoustics
images: images/pyroomacoustics.png
links:
  - icon: file
    url: https://arxiv.org/abs/1710.04196
  - icon: github
    url: https://github.com/LCAV/pyroomacoustics
hidden: true
---

[Pyroomacoustics](https://github.com/LCAV/pyroomacoustics) is a software
package aimed at the rapid development and testing of audio array processing
algorithms. The content of the package can be divided into three main
components. 

* An intuitive Python object-oriented
  interface to quickly construct different simulation scenarios involving
  multiple sound sources and microphones in 2D and 3D rooms; 
* A fast C implementation of the image source model for general polyhedral rooms to
  efficiently generate room impulse responses and simulate the propagation
  between sources and receivers; 
* Reference implementations of popular algorithms for beamforming, direction
  finding, and adaptive filtering.  Together, they form a package with the
  potential to speed up the time to market of new algorithms by significantly
  reducing the implementation overhead in the performance evaluation step.

Check out [our paper](https://arxiv.org/abs/1710.04196) describing the package.
