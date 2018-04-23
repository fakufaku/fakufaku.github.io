---
title: Echo-aware Audio Processing
layout: project
tagline: "Echoes are our friends"
description: "Like in human audition, early echoes improve the output from audio processing algorithms."
klass: audio
permalink: /raking
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

This is a joint research project with Ivan Dokmani\'{c} (UIUC), Antoine
Deleforge (INRIA), Diego Di Carlo (INRIA).  We hope to promote further the
appreciation for echoes by applying similar ideas to scene analysis and
recognition tasks for example.

Acoustic Rake Receivers
-----------------------

Beamformers combine the signal from multiple microphones to focus the
acquisition towards some regions of space. We propose a number of beamforming
algorithms that maximize some well-defined criteria that include echoes. This
results in the created beams to focus not only on the direct sound, but also
towards strong reflections on walls.  This enable some previously impossible
tasks such as listening _behind_ an interferer placed between the microphones
and the target source. This is effectively done by steering the beams towards
the reflections on the walls, ignoring the direct path completely.

The code is available on github for [frequency
domain](https://github.com/LCAV/AcousticRakeReceiver) and [time
domain](https://github.com/LCAV/TimeDomainAcousticRakeReceiver).  The papers
are [here](http://ieeexplore.ieee.org/document/7065205/) and
[here](https://github.com/LCAV/TimeDomainAcousticRakeReceiver).

Separake
--------

More recently, we showed similar results in the domain of
source separation.  Here we use non-negative models of the spectrogram and a
well known algorithm for their separation. While the original algorithm
attempts the estimation of the room impulse responses (RIR) together with
the separation of the speeches, we assume the knowledge of one to five
echoes and use that to form a poor man's estimate of the RIR. We then
discovered that using even a single  echo outperforms the fully blind
approach. Adding more echoes, only then improves things further.

The code is available on [github](https://github.com/fakufaku/separake) and
sound samples are below. The paper is [here](https://arxiv.org/abs/1711.06805).

<style type="text/css">
audio {
  width: 50px;
}
</style>

<table>
  <tr>
  <td colspan="2"></td>
  <td colspan="2">MU-NMF Spkr Dep</td>
  <td colspan="2">EM-NMF Spkr Dep</td>
  <td colspan="2">MU-NMF Universal</td>
  </tr>

  <tr>
  <td></td>
  <td>Mix</td>
  <td>Male</td>
  <td>Female</td>
  <td>Male</td>
  <td>Female</td>
  <td>Male</td>
  <td>Female</td>
  </tr>

  <tr>
  <td>Anechoic</td>

  <td><audio controls="controls" type="audio/wav" src="/assets/samples/separake_anechoic_mu_spkr_mix_fq_sample3_fq_sample2.wav"><a>play</a></audio></td>

  <td><audio controls="controls" type="audio/wav" src="/assets/samples/separake_anechoic_mu_spkr_sep_fq_sample2.wav"><a>play</a></audio></td>
  <td><audio controls="controls" type="audio/wav" src="/assets/samples/separake_anechoic_mu_spkr_sep_fq_sample3.wav"><a>play</a></audio></td>

  <td><audio controls="controls" type="audio/wav" src="/assets/samples/separake_anechoic_em_spkr_sep_fq_sample2.wav"><a>play</a></audio></td>
  <td><audio controls="controls" type="audio/wav" src="/assets/samples/separake_anechoic_em_spkr_sep_fq_sample3.wav"><a>play</a></audio></td>

  <td><audio controls="controls" type="audio/wav" src="/assets/samples/separake_anechoic_mu_univ_sep_fq_sample2.wav"><a>play</a></audio></td>
  <td><audio controls="controls" type="audio/wav" src="/assets/samples/separake_anechoic_mu_univ_sep_fq_sample3.wav"><a>play</a></audio></td>
  </tr>

  <tr>
  <td>Learn</td>

  <td><audio controls="controls" type="audio/wav" src="/assets/samples/separake_learn_mu_spkr_mix_fq_sample3_fq_sample2.wav"><a>play</a></audio></td>

  <td><audio controls="controls" type="audio/wav" src="/assets/samples/separake_learn_mu_spkr_sep_fq_sample2.wav"><a>play</a></audio></td>
  <td><audio controls="controls" type="audio/wav" src="/assets/samples/separake_learn_mu_spkr_sep_fq_sample3.wav"><a>play</a></audio></td>

  <td><audio controls="controls" type="audio/wav" src="/assets/samples/separake_learn_em_spkr_sep_fq_sample2.wav"><a>play</a></audio></td>
  <td><audio controls="controls" type="audio/wav" src="/assets/samples/separake_learn_em_spkr_sep_fq_sample3.wav"><a>play</a></audio></td>

  <td><audio controls="controls" type="audio/wav" src="/assets/samples/separake_learn_mu_univ_sep_fq_sample2.wav"><a>play</a></audio></td>
  <td><audio controls="controls" type="audio/wav" src="/assets/samples/separake_learn_mu_univ_sep_fq_sample3.wav"><a>play</a></audio></td>
  </tr>
  
  <tr>
  <td>0 Echoes</td>
  <td><audio controls="controls" type="audio/wav" src="/assets/samples/separake_learn_mu_spkr_mix_fq_sample3_fq_sample2.wav"><a>play</a></audio></td>

  <td><audio controls="controls" type="audio/wav" src="/assets/samples/separake_0echoes_mu_spkr_sep_fq_sample2.wav"><a>play</a></audio></td>
  <td><audio controls="controls" type="audio/wav" src="/assets/samples/separake_0echoes_mu_spkr_sep_fq_sample3.wav"><a>play</a></audio></td>

  <td><audio controls="controls" type="audio/wav" src="/assets/samples/separake_0echoes_em_spkr_sep_fq_sample2.wav"><a>play</a></audio></td>
  <td><audio controls="controls" type="audio/wav" src="/assets/samples/separake_0echoes_em_spkr_sep_fq_sample3.wav"><a>play</a></audio></td>

  <td><audio controls="controls" type="audio/wav" src="/assets/samples/separake_0echoes_mu_univ_sep_fq_sample2.wav"><a>play</a></audio></td>
  <td><audio controls="controls" type="audio/wav" src="/assets/samples/separake_0echoes_mu_univ_sep_fq_sample3.wav"><a>play</a></audio></td>
  </tr>
  
  <tr>
  <td>1 Echoes</td>
  <td><audio controls="controls" type="audio/wav" src="/assets/samples/separake_learn_mu_spkr_mix_fq_sample3_fq_sample2.wav"><a>play</a></audio></td>

  <td><audio controls="controls" type="audio/wav" src="/assets/samples/separake_1echoes_mu_spkr_sep_fq_sample2.wav"><a>play</a></audio></td>
  <td><audio controls="controls" type="audio/wav" src="/assets/samples/separake_1echoes_mu_spkr_sep_fq_sample3.wav"><a>play</a></audio></td>

  <td><audio controls="controls" type="audio/wav" src="/assets/samples/separake_1echoes_em_spkr_sep_fq_sample2.wav"><a>play</a></audio></td>
  <td><audio controls="controls" type="audio/wav" src="/assets/samples/separake_1echoes_em_spkr_sep_fq_sample3.wav"><a>play</a></audio></td>

  <td><audio controls="controls" type="audio/wav" src="/assets/samples/separake_1echoes_mu_univ_sep_fq_sample2.wav"><a>play</a></audio></td>
  <td><audio controls="controls" type="audio/wav" src="/assets/samples/separake_1echoes_mu_univ_sep_fq_sample3.wav"><a>play</a></audio></td>
  </tr>

  <tr>
  <td>2 Echoes</td>
  <td><audio controls="controls" type="audio/wav" src="/assets/samples/separake_anechoic_em_spkr_mix_fq_sample3_fq_sample2.wav"><a>play</a></audio></td>

  <td><audio controls="controls" type="audio/wav" src="/assets/samples/separake_2echoes_mu_spkr_sep_fq_sample2.wav"><a>play</a></audio></td>
  <td><audio controls="controls" type="audio/wav" src="/assets/samples/separake_2echoes_mu_spkr_sep_fq_sample3.wav"><a>play</a></audio></td>

  <td><audio controls="controls" type="audio/wav" src="/assets/samples/separake_2echoes_em_spkr_sep_fq_sample2.wav"><a>play</a></audio></td>
  <td><audio controls="controls" type="audio/wav" src="/assets/samples/separake_2echoes_em_spkr_sep_fq_sample3.wav"><a>play</a></audio></td>

  <td><audio controls="controls" type="audio/wav" src="/assets/samples/separake_2echoes_mu_univ_sep_fq_sample2.wav"><a>play</a></audio></td>
  <td><audio controls="controls" type="audio/wav" src="/assets/samples/separake_2echoes_mu_univ_sep_fq_sample3.wav"><a>play</a></audio></td>
  </tr>

  <tr>
  <td>3 Echoes</td>
  <td><audio controls="controls" type="audio/wav" src="/assets/samples/separake_learn_mu_univ_mix_fq_sample3_fq_sample2.wav"><a>play</a></audio></td>

  <td><audio controls="controls" type="audio/wav" src="/assets/samples/separake_3echoes_mu_spkr_sep_fq_sample2.wav"><a>play</a></audio></td>
  <td><audio controls="controls" type="audio/wav" src="/assets/samples/separake_3echoes_mu_spkr_sep_fq_sample3.wav"><a>play</a></audio></td>

  <td><audio controls="controls" type="audio/wav" src="/assets/samples/separake_3echoes_em_spkr_sep_fq_sample2.wav"><a>play</a></audio></td>
  <td><audio controls="controls" type="audio/wav" src="/assets/samples/separake_3echoes_em_spkr_sep_fq_sample3.wav"><a>play</a></audio></td>

  <td><audio controls="controls" type="audio/wav" src="/assets/samples/separake_3echoes_mu_univ_sep_fq_sample2.wav"><a>play</a></audio></td>
  <td><audio controls="controls" type="audio/wav" src="/assets/samples/separake_3echoes_mu_univ_sep_fq_sample3.wav"><a>play</a></audio></td>
  </tr>
</table>
