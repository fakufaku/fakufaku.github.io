---
title: Pyroomacoustics
layout: project
tagline: "Fast image sources and array processing algorithms"
description: "A python package providing fast image source model for shoebox and polygonal rooms."
klass: software
permalink: /pyroomacoustics
images: images/pyroomacoustics.png
pdf: https://arxiv.org/abs/1710.04196
repo: https://github.com/LCAV/pyroomacoustics
hidden: true
---

The sparse fast Hadamard transform is a new iterative low-complexity algorithm for computing
the Walsh-Hadamard transform (WHT) of an N dimensional signal with a K-sparse
WHT.  We suppose that N is a power of two and K = O(Nα), scales sub-linearly in
N for some α ∈ (0,1). Assuming a random support model for the nonzero
transform-domain components, our algorithm reconstructs the WHT of the signal
with a sample complexity O(K log ( N )) and a computational complexity N2K O(K
log2(K)log2(K )). Moreover, the algorithm succeeds with a high probability
approaching 1 for large dimension N.  Our approach is mainly based on the
subsampling (aliasing) property of the WHT, where by a carefully designed
subsampling of the time-domain signal, a suitable aliasing pattern is induced
in the transform-domain. We treat the resulting aliasing patterns as
parity-check constraints and represent them by a bipartite graph.  We analyze
the properties of the resulting bipartite graphs and borrow ideas from codes
defined over sparse bipartite graphs to formulate the recovery of the nonzero
spectral values as a peeling decoding algorithm for a specific sparse-graph
code transmitted over a binary erasure channel (BEC). This enables us to use
tools from coding theory (belief-propagation analysis) to characterize the
asymptotic performance of our algorithm in the very sparse (α ∈ (0,1]) and the
less sparse (α ∈ (1,1)) 33 regime. Comprehensive simulation results are
provided to assess the empirical performance of the proposed algorithm.
