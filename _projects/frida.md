---
title: FRIDA -- Robust DOA Finding
layout: project
tagline: "Finite Rate of Innovation - Direction of Arrival"
description: "A robust parametric DOA finding algorithm."
klass: audio
images: images/frida.png
hidden: true
---

Finite-rate of innovation (FRI) is a framework for the estimation of sparse continuous signals.
Oftentime, audio sources are sparse into space and we exploit this feature to apply
the FRI framework to the DOA estimation problem. Contrary to previous work on the topic,
our algorithm works reliably with arbitrary microphone array geometry, uses multiband
information and can handle both 2D (azimuth only) and full 3D localization.
A real-time implementation of the algorithm was demonstrated multiple times using the CompactSix
and Pyramic arrays.
