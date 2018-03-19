---
title: Echo-aware Audio Processing
layout: project
tagline: "Echoes are our friends"
description: "Like in human audition, early echoes improve the output from audio processing algorithms."
klass: audio
images: images/rake.png
links:
  - icon: book
    url: http://ieeexplore.ieee.org/document/7065205/
  - icon: github
    url: https://github.com/LCAV/AcousticRakeReceiver
hidden: true
---

Research in psychoacoustics has shown that early echoes arriving within 30 to
90 ms of the direct sound improve intelligibility. Building on the intuition
that what is true in humans might be true for audio processing in general, we
augment a number of classic algorithms by including the knowledge of a few
early echoes in their design. We then provide evidence that algorithms
including echoes perform better than those ignoring or suppressing them.

1. **Raking Beamformers**: Beamformers combine the signal from multiple
   microphones to focus the acquisition towards some regions of space. We
   propose a number of beamforming algorithms that maximize some well-defined
   criteria that include echoes. This results in the created beams to focus not
   only on the direct sound, but also towards strong reflections on walls.
   This enable some previously impossible tasks such as listening _behind_ an
   interferer placed between the microphones and the target source. This is
   effectively done by steering the beams towards the reflections on the walls,
   ignoring the direct path completely.

2. **Separake**: More recently, we showed similar results in the domain of
   source separation.  Here we use non-negative models of the spectrogram and a
   well known algorithm for their separation. While the original algorithm
   attempts the estimation of the room impulse responses (RIR) together with
   the separation of the speeches, we assume the knowledge of one to five
   echoes and use that to form a poor man's estimate of the RIR. We then
   discovered that using even a single  echo outperforms the fully blind
   approach. Adding more echoes, only then improves things further.

This is a joint research project with Ivan Dokmani\'{c} (UIUC), Antoine
Deleforge (INRIA), Diego Di Carlo (INRIA).  We hope to promote further the
appreciation for echoes by applying similar ideas to scene analysis and
recognition tasks for example.
