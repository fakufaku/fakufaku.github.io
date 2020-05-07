---
title: "ICASSP 2020"
layout: project
tagline: "Fast Independent Vector Extraction"
description: "Audio samples for our publications at ICASSP 2020"
permalink: /icassp2020
klass: audio
images: assets/icassp2020/images/icassp2020_logo.png
hidden: true
---

## Fast Independent Vector Extraction by Iterative SINR Maximization

### Abstract

We propose fast independent vector extraction (FIVE), a new algorithm that
blindly extracts a single non-Gaussian source from a Gaussian background. The
algorithm iteratively computes beamforming weights maximizing the
signal-to-interference-and-noise ratio for an approximate noise covariance
matrix. We demonstrate that this procedure minimizes the negative
log-likelihood of the input data according to a well-defined probabilistic
model. The minimization is carried out via the auxiliary function technique
whereas, unlike related methods, the auxiliary function is globally minimized
at every iteration. Numerical experiments are carried out to assess the
performance of FIVE. We find that it is vastly superior to competing methods in
terms of convergence speed, and has high potential for real-time applications.

## Audio Samples

The algorithms are
* FIVE: The proposed method.
* OverIVA: Our previous method [Scheibler and Ono, WASPAA 2019]
* AuxIVA: Full blind source separation with AuxIVA [Ono, WASPAA 2011], selection of output source with largest power

The signal-to-interference and noise ratio is fixed to 5 dB. The source model is time-varying Gaussian.

<style type="text/css">
audio {
width: 50px;
}
</style>

<table>
  <tr>
    <td>mics</td>
    <td>sample</td>
    <td>algo.</td>
    <td>clean</td>
    <td>mix</td>
    <td>output</td>
    <td>SDR</td>
    <td>SIR</td>
    <td>iter.</td>
    <td>runtime</td>
  </tr>
  <tr>
    <td>2</td>
    <td>1</td>
    <td>FIVE</td>
    <td><audio controls="controls" type="audio/wav" src="/assets/icassp2020/samples/sample_5_2785643_five_gauss_2_ref.wav"><a>play</a></audio></td>
    <td><audio controls="controls" type="audio/wav" src="/assets/icassp2020/samples/sample_5_2785643_five_gauss_2_mix.wav"><a>play</a></audio></td>
    <td><audio controls="controls" type="audio/wav" src="/assets/icassp2020/samples/sample_5_2785643_five_gauss_2_source0.wav"><a>play</a></audio></td>
    <td>9.00 dB</td>
    <td>12.84 dB</td>
    <td>3</td>
    <td>0.131 s</td>
  </tr>
  <tr>
    <td>2</td>
    <td>1</td>
    <td>OverIVA</td>
    <td><audio controls="controls" type="audio/wav" src="/assets/icassp2020/samples/sample_5_2785643_overiva_gauss_2_ref.wav"><a>play</a></audio></td>
    <td><audio controls="controls" type="audio/wav" src="/assets/icassp2020/samples/sample_5_2785643_overiva_gauss_2_mix.wav"><a>play</a></audio></td>
    <td><audio controls="controls" type="audio/wav" src="/assets/icassp2020/samples/sample_5_2785643_overiva_gauss_2_source0.wav"><a>play</a></audio></td>
    <td>8.95 dB</td>
    <td>12.84 dB</td>
    <td>10</td>
    <td>0.234 s</td>
  </tr>
  <tr>
    <td>2</td>
    <td>1</td>
    <td>AuxIVA</td>
    <td><audio controls="controls" type="audio/wav" src="/assets/icassp2020/samples/sample_5_2785643_auxiva_gauss_2_ref.wav"><a>play</a></audio></td>
    <td><audio controls="controls" type="audio/wav" src="/assets/icassp2020/samples/sample_5_2785643_auxiva_gauss_2_mix.wav"><a>play</a></audio></td>
    <td><audio controls="controls" type="audio/wav" src="/assets/icassp2020/samples/sample_5_2785643_auxiva_gauss_2_source0.wav"><a>play</a></audio></td>
    <td>9.20 dB</td>
    <td>13.21 dB</td>
    <td>50</td>
    <td>2.047 s</td>
  </tr>
  <tr>
    <td>2</td>
    <td>2</td>
    <td>FIVE</td>
    <td><audio controls="controls" type="audio/wav" src="/assets/icassp2020/samples/sample_5_398745627_five_gauss_2_ref.wav"><a>play</a></audio></td>
    <td><audio controls="controls" type="audio/wav" src="/assets/icassp2020/samples/sample_5_398745627_five_gauss_2_mix.wav"><a>play</a></audio></td>
    <td><audio controls="controls" type="audio/wav" src="/assets/icassp2020/samples/sample_5_398745627_five_gauss_2_source0.wav"><a>play</a></audio></td>
    <td>4.93 dB</td>
    <td>8.99 dB</td>
    <td>3</td>
    <td>0.198 s</td>
  </tr>
  <tr>
    <td>2</td>
    <td>2</td>
    <td>OverIVA</td>
    <td><audio controls="controls" type="audio/wav" src="/assets/icassp2020/samples/sample_5_398745627_overiva_gauss_2_ref.wav"><a>play</a></audio></td>
    <td><audio controls="controls" type="audio/wav" src="/assets/icassp2020/samples/sample_5_398745627_overiva_gauss_2_mix.wav"><a>play</a></audio></td>
    <td><audio controls="controls" type="audio/wav" src="/assets/icassp2020/samples/sample_5_398745627_overiva_gauss_2_source0.wav"><a>play</a></audio></td>
    <td>4.33 dB</td>
    <td>8.26 dB</td>
    <td>10</td>
    <td>0.324 s</td>
  </tr>
  <tr>
    <td>2</td>
    <td>2</td>
    <td>AuxIVA</td>
    <td><audio controls="controls" type="audio/wav" src="/assets/icassp2020/samples/sample_5_398745627_auxiva_gauss_2_ref.wav"><a>play</a></audio></td>
    <td><audio controls="controls" type="audio/wav" src="/assets/icassp2020/samples/sample_5_398745627_auxiva_gauss_2_mix.wav"><a>play</a></audio></td>
    <td><audio controls="controls" type="audio/wav" src="/assets/icassp2020/samples/sample_5_398745627_auxiva_gauss_2_source0.wav"><a>play</a></audio></td>
    <td>7.27 dB</td>
    <td>11.46 dB</td>
    <td>50</td>
    <td>2.427 s</td>
  </tr>
  <tr>
    <td>2</td>
    <td>3</td>
    <td>FIVE</td>
    <td><audio controls="controls" type="audio/wav" src="/assets/icassp2020/samples/sample_5_58984517_five_gauss_2_ref.wav"><a>play</a></audio></td>
    <td><audio controls="controls" type="audio/wav" src="/assets/icassp2020/samples/sample_5_58984517_five_gauss_2_mix.wav"><a>play</a></audio></td>
    <td><audio controls="controls" type="audio/wav" src="/assets/icassp2020/samples/sample_5_58984517_five_gauss_2_source0.wav"><a>play</a></audio></td>
    <td>7.44 dB</td>
    <td>10.85 dB</td>
    <td>3</td>
    <td>0.168 s</td>
  </tr>
  <tr>
    <td>2</td>
    <td>3</td>
    <td>OverIVA</td>
    <td><audio controls="controls" type="audio/wav" src="/assets/icassp2020/samples/sample_5_58984517_overiva_gauss_2_ref.wav"><a>play</a></audio></td>
    <td><audio controls="controls" type="audio/wav" src="/assets/icassp2020/samples/sample_5_58984517_overiva_gauss_2_mix.wav"><a>play</a></audio></td>
    <td><audio controls="controls" type="audio/wav" src="/assets/icassp2020/samples/sample_5_58984517_overiva_gauss_2_source0.wav"><a>play</a></audio></td>
    <td>7.22 dB</td>
    <td>10.44 dB</td>
    <td>10</td>
    <td>0.230 s</td>
  </tr>
  <tr>
    <td>2</td>
    <td>3</td>
    <td>AuxIVA</td>
    <td><audio controls="controls" type="audio/wav" src="/assets/icassp2020/samples/sample_5_58984517_auxiva_gauss_2_ref.wav"><a>play</a></audio></td>
    <td><audio controls="controls" type="audio/wav" src="/assets/icassp2020/samples/sample_5_58984517_auxiva_gauss_2_mix.wav"><a>play</a></audio></td>
    <td><audio controls="controls" type="audio/wav" src="/assets/icassp2020/samples/sample_5_58984517_auxiva_gauss_2_source0.wav"><a>play</a></audio></td>
    <td>7.30 dB</td>
    <td>10.64 dB</td>
    <td>50</td>
    <td>1.625 s</td>
  </tr>
  <tr>
    <td>3</td>
    <td>1</td>
    <td>FIVE</td>
    <td><audio controls="controls" type="audio/wav" src="/assets/icassp2020/samples/sample_5_2785643_five_gauss_3_ref.wav"><a>play</a></audio></td>
    <td><audio controls="controls" type="audio/wav" src="/assets/icassp2020/samples/sample_5_2785643_five_gauss_3_mix.wav"><a>play</a></audio></td>
    <td><audio controls="controls" type="audio/wav" src="/assets/icassp2020/samples/sample_5_2785643_five_gauss_3_source0.wav"><a>play</a></audio></td>
    <td>12.09 dB</td>
    <td>18.01 dB</td>
    <td>3</td>
    <td>0.217 s</td>
  </tr>
  <tr>
    <td>3</td>
    <td>1</td>
    <td>OverIVA</td>
    <td><audio controls="controls" type="audio/wav" src="/assets/icassp2020/samples/sample_5_2785643_overiva_gauss_3_ref.wav"><a>play</a></audio></td>
    <td><audio controls="controls" type="audio/wav" src="/assets/icassp2020/samples/sample_5_2785643_overiva_gauss_3_mix.wav"><a>play</a></audio></td>
    <td><audio controls="controls" type="audio/wav" src="/assets/icassp2020/samples/sample_5_2785643_overiva_gauss_3_source0.wav"><a>play</a></audio></td>
    <td>12.08 dB</td>
    <td>18.36 dB</td>
    <td>10</td>
    <td>0.294 s</td>
  </tr>
  <tr>
    <td>3</td>
    <td>1</td>
    <td>AuxIVA</td>
    <td><audio controls="controls" type="audio/wav" src="/assets/icassp2020/samples/sample_5_2785643_auxiva_gauss_3_ref.wav"><a>play</a></audio></td>
    <td><audio controls="controls" type="audio/wav" src="/assets/icassp2020/samples/sample_5_2785643_auxiva_gauss_3_mix.wav"><a>play</a></audio></td>
    <td><audio controls="controls" type="audio/wav" src="/assets/icassp2020/samples/sample_5_2785643_auxiva_gauss_3_source0.wav"><a>play</a></audio></td>
    <td>12.68 dB</td>
    <td>20.50 dB</td>
    <td>50</td>
    <td>3.365 s</td>
  </tr>
  <tr>
    <td>3</td>
    <td>2</td>
    <td>FIVE</td>
    <td><audio controls="controls" type="audio/wav" src="/assets/icassp2020/samples/sample_5_398745627_five_gauss_3_ref.wav"><a>play</a></audio></td>
    <td><audio controls="controls" type="audio/wav" src="/assets/icassp2020/samples/sample_5_398745627_five_gauss_3_mix.wav"><a>play</a></audio></td>
    <td><audio controls="controls" type="audio/wav" src="/assets/icassp2020/samples/sample_5_398745627_five_gauss_3_source0.wav"><a>play</a></audio></td>
    <td>7.80 dB</td>
    <td>13.99 dB</td>
    <td>3</td>
    <td>0.199 s</td>
  </tr>
  <tr>
    <td>3</td>
    <td>2</td>
    <td>OverIVA</td>
    <td><audio controls="controls" type="audio/wav" src="/assets/icassp2020/samples/sample_5_398745627_overiva_gauss_3_ref.wav"><a>play</a></audio></td>
    <td><audio controls="controls" type="audio/wav" src="/assets/icassp2020/samples/sample_5_398745627_overiva_gauss_3_mix.wav"><a>play</a></audio></td>
    <td><audio controls="controls" type="audio/wav" src="/assets/icassp2020/samples/sample_5_398745627_overiva_gauss_3_source0.wav"><a>play</a></audio></td>
    <td>6.83 dB</td>
    <td>12.86 dB</td>
    <td>10</td>
    <td>0.366 s</td>
  </tr>
  <tr>
    <td>3</td>
    <td>2</td>
    <td>AuxIVA</td>
    <td><audio controls="controls" type="audio/wav" src="/assets/icassp2020/samples/sample_5_398745627_auxiva_gauss_3_ref.wav"><a>play</a></audio></td>
    <td><audio controls="controls" type="audio/wav" src="/assets/icassp2020/samples/sample_5_398745627_auxiva_gauss_3_mix.wav"><a>play</a></audio></td>
    <td><audio controls="controls" type="audio/wav" src="/assets/icassp2020/samples/sample_5_398745627_auxiva_gauss_3_source0.wav"><a>play</a></audio></td>
    <td>9.78 dB</td>
    <td>18.10 dB</td>
    <td>50</td>
    <td>3.145 s</td>
  </tr>
  <tr>
    <td>3</td>
    <td>3</td>
    <td>FIVE</td>
    <td><audio controls="controls" type="audio/wav" src="/assets/icassp2020/samples/sample_5_58984517_five_gauss_3_ref.wav"><a>play</a></audio></td>
    <td><audio controls="controls" type="audio/wav" src="/assets/icassp2020/samples/sample_5_58984517_five_gauss_3_mix.wav"><a>play</a></audio></td>
    <td><audio controls="controls" type="audio/wav" src="/assets/icassp2020/samples/sample_5_58984517_five_gauss_3_source0.wav"><a>play</a></audio></td>
    <td>11.05 dB</td>
    <td>17.21 dB</td>
    <td>3</td>
    <td>0.236 s</td>
  </tr>
  <tr>
    <td>3</td>
    <td>3</td>
    <td>OverIVA</td>
    <td><audio controls="controls" type="audio/wav" src="/assets/icassp2020/samples/sample_5_58984517_overiva_gauss_3_ref.wav"><a>play</a></audio></td>
    <td><audio controls="controls" type="audio/wav" src="/assets/icassp2020/samples/sample_5_58984517_overiva_gauss_3_mix.wav"><a>play</a></audio></td>
    <td><audio controls="controls" type="audio/wav" src="/assets/icassp2020/samples/sample_5_58984517_overiva_gauss_3_source0.wav"><a>play</a></audio></td>
    <td>10.74 dB</td>
    <td>16.67 dB</td>
    <td>10</td>
    <td>0.318 s</td>
  </tr>
  <tr>
    <td>3</td>
    <td>3</td>
    <td>AuxIVA</td>
    <td><audio controls="controls" type="audio/wav" src="/assets/icassp2020/samples/sample_5_58984517_auxiva_gauss_3_ref.wav"><a>play</a></audio></td>
    <td><audio controls="controls" type="audio/wav" src="/assets/icassp2020/samples/sample_5_58984517_auxiva_gauss_3_mix.wav"><a>play</a></audio></td>
    <td><audio controls="controls" type="audio/wav" src="/assets/icassp2020/samples/sample_5_58984517_auxiva_gauss_3_source0.wav"><a>play</a></audio></td>
    <td>10.55 dB</td>
    <td>16.40 dB</td>
    <td>50</td>
    <td>3.989 s</td>
  </tr>
  <tr>
    <td>5</td>
    <td>1</td>
    <td>FIVE</td>
    <td><audio controls="controls" type="audio/wav" src="/assets/icassp2020/samples/sample_5_2785643_five_gauss_5_ref.wav"><a>play</a></audio></td>
    <td><audio controls="controls" type="audio/wav" src="/assets/icassp2020/samples/sample_5_2785643_five_gauss_5_mix.wav"><a>play</a></audio></td>
    <td><audio controls="controls" type="audio/wav" src="/assets/icassp2020/samples/sample_5_2785643_five_gauss_5_source0.wav"><a>play</a></audio></td>
    <td>15.60 dB</td>
    <td>22.01 dB</td>
    <td>3</td>
    <td>0.416 s</td>
  </tr>
  <tr>
    <td>5</td>
    <td>1</td>
    <td>OverIVA</td>
    <td><audio controls="controls" type="audio/wav" src="/assets/icassp2020/samples/sample_5_2785643_overiva_gauss_5_ref.wav"><a>play</a></audio></td>
    <td><audio controls="controls" type="audio/wav" src="/assets/icassp2020/samples/sample_5_2785643_overiva_gauss_5_mix.wav"><a>play</a></audio></td>
    <td><audio controls="controls" type="audio/wav" src="/assets/icassp2020/samples/sample_5_2785643_overiva_gauss_5_source0.wav"><a>play</a></audio></td>
    <td>15.72 dB</td>
    <td>23.63 dB</td>
    <td>10</td>
    <td>0.574 s</td>
  </tr>
  <tr>
    <td>5</td>
    <td>1</td>
    <td>AuxIVA</td>
    <td><audio controls="controls" type="audio/wav" src="/assets/icassp2020/samples/sample_5_2785643_auxiva_gauss_5_ref.wav"><a>play</a></audio></td>
    <td><audio controls="controls" type="audio/wav" src="/assets/icassp2020/samples/sample_5_2785643_auxiva_gauss_5_mix.wav"><a>play</a></audio></td>
    <td><audio controls="controls" type="audio/wav" src="/assets/icassp2020/samples/sample_5_2785643_auxiva_gauss_5_source0.wav"><a>play</a></audio></td>
    <td>16.29 dB</td>
    <td>30.70 dB</td>
    <td>50</td>
    <td>9.467 s</td>
  </tr>
  <tr>
    <td>5</td>
    <td>2</td>
    <td>FIVE</td>
    <td><audio controls="controls" type="audio/wav" src="/assets/icassp2020/samples/sample_5_398745627_five_gauss_5_ref.wav"><a>play</a></audio></td>
    <td><audio controls="controls" type="audio/wav" src="/assets/icassp2020/samples/sample_5_398745627_five_gauss_5_mix.wav"><a>play</a></audio></td>
    <td><audio controls="controls" type="audio/wav" src="/assets/icassp2020/samples/sample_5_398745627_five_gauss_5_source0.wav"><a>play</a></audio></td>
    <td>10.94 dB</td>
    <td>19.25 dB</td>
    <td>3</td>
    <td>0.374 s</td>
  </tr>
  <tr>
    <td>5</td>
    <td>2</td>
    <td>OverIVA</td>
    <td><audio controls="controls" type="audio/wav" src="/assets/icassp2020/samples/sample_5_398745627_overiva_gauss_5_ref.wav"><a>play</a></audio></td>
    <td><audio controls="controls" type="audio/wav" src="/assets/icassp2020/samples/sample_5_398745627_overiva_gauss_5_mix.wav"><a>play</a></audio></td>
    <td><audio controls="controls" type="audio/wav" src="/assets/icassp2020/samples/sample_5_398745627_overiva_gauss_5_source0.wav"><a>play</a></audio></td>
    <td>10.13 dB</td>
    <td>19.04 dB</td>
    <td>10</td>
    <td>0.590 s</td>
  </tr>
  <tr>
    <td>5</td>
    <td>2</td>
    <td>AuxIVA</td>
    <td><audio controls="controls" type="audio/wav" src="/assets/icassp2020/samples/sample_5_398745627_auxiva_gauss_5_ref.wav"><a>play</a></audio></td>
    <td><audio controls="controls" type="audio/wav" src="/assets/icassp2020/samples/sample_5_398745627_auxiva_gauss_5_mix.wav"><a>play</a></audio></td>
    <td><audio controls="controls" type="audio/wav" src="/assets/icassp2020/samples/sample_5_398745627_auxiva_gauss_5_source0.wav"><a>play</a></audio></td>
    <td>9.76 dB</td>
    <td>24.72 dB</td>
    <td>50</td>
    <td>10.101 s</td>
  </tr>
  <tr>
    <td>5</td>
    <td>3</td>
    <td>FIVE</td>
    <td><audio controls="controls" type="audio/wav" src="/assets/icassp2020/samples/sample_5_58984517_five_gauss_5_ref.wav"><a>play</a></audio></td>
    <td><audio controls="controls" type="audio/wav" src="/assets/icassp2020/samples/sample_5_58984517_five_gauss_5_mix.wav"><a>play</a></audio></td>
    <td><audio controls="controls" type="audio/wav" src="/assets/icassp2020/samples/sample_5_58984517_five_gauss_5_source0.wav"><a>play</a></audio></td>
    <td>13.30 dB</td>
    <td>19.85 dB</td>
    <td>3</td>
    <td>0.371 s</td>
  </tr>
  <tr>
    <td>5</td>
    <td>3</td>
    <td>OverIVA</td>
    <td><audio controls="controls" type="audio/wav" src="/assets/icassp2020/samples/sample_5_58984517_overiva_gauss_5_ref.wav"><a>play</a></audio></td>
    <td><audio controls="controls" type="audio/wav" src="/assets/icassp2020/samples/sample_5_58984517_overiva_gauss_5_mix.wav"><a>play</a></audio></td>
    <td><audio controls="controls" type="audio/wav" src="/assets/icassp2020/samples/sample_5_58984517_overiva_gauss_5_source0.wav"><a>play</a></audio></td>
    <td>12.86 dB</td>
    <td>19.71 dB</td>
    <td>10</td>
    <td>0.641 s</td>
  </tr>
  <tr>
    <td>5</td>
    <td>3</td>
    <td>AuxIVA</td>
    <td><audio controls="controls" type="audio/wav" src="/assets/icassp2020/samples/sample_5_58984517_auxiva_gauss_5_ref.wav"><a>play</a></audio></td>
    <td><audio controls="controls" type="audio/wav" src="/assets/icassp2020/samples/sample_5_58984517_auxiva_gauss_5_mix.wav"><a>play</a></audio></td>
    <td><audio controls="controls" type="audio/wav" src="/assets/icassp2020/samples/sample_5_58984517_auxiva_gauss_5_source0.wav"><a>play</a></audio></td>
    <td>13.97 dB</td>
    <td>22.14 dB</td>
    <td>50</td>
    <td>9.901 s</td>
  </tr>
  <tr>
    <td>8</td>
    <td>1</td>
    <td>FIVE</td>
    <td><audio controls="controls" type="audio/wav" src="/assets/icassp2020/samples/sample_5_2785643_five_gauss_8_ref.wav"><a>play</a></audio></td>
    <td><audio controls="controls" type="audio/wav" src="/assets/icassp2020/samples/sample_5_2785643_five_gauss_8_mix.wav"><a>play</a></audio></td>
    <td><audio controls="controls" type="audio/wav" src="/assets/icassp2020/samples/sample_5_2785643_five_gauss_8_source0.wav"><a>play</a></audio></td>
    <td>16.49 dB</td>
    <td>23.89 dB</td>
    <td>3</td>
    <td>0.633 s</td>
  </tr>
  <tr>
    <td>8</td>
    <td>1</td>
    <td>OverIVA</td>
    <td><audio controls="controls" type="audio/wav" src="/assets/icassp2020/samples/sample_5_2785643_overiva_gauss_8_ref.wav"><a>play</a></audio></td>
    <td><audio controls="controls" type="audio/wav" src="/assets/icassp2020/samples/sample_5_2785643_overiva_gauss_8_mix.wav"><a>play</a></audio></td>
    <td><audio controls="controls" type="audio/wav" src="/assets/icassp2020/samples/sample_5_2785643_overiva_gauss_8_source0.wav"><a>play</a></audio></td>
    <td>17.40 dB</td>
    <td>31.68 dB</td>
    <td>10</td>
    <td>0.910 s</td>
  </tr>
  <tr>
    <td>8</td>
    <td>1</td>
    <td>AuxIVA</td>
    <td><audio controls="controls" type="audio/wav" src="/assets/icassp2020/samples/sample_5_2785643_auxiva_gauss_8_ref.wav"><a>play</a></audio></td>
    <td><audio controls="controls" type="audio/wav" src="/assets/icassp2020/samples/sample_5_2785643_auxiva_gauss_8_mix.wav"><a>play</a></audio></td>
    <td><audio controls="controls" type="audio/wav" src="/assets/icassp2020/samples/sample_5_2785643_auxiva_gauss_8_source0.wav"><a>play</a></audio></td>
    <td>17.50 dB</td>
    <td>33.20 dB</td>
    <td>50</td>
    <td>22.396 s</td>
  </tr>
  <tr>
    <td>8</td>
    <td>2</td>
    <td>FIVE</td>
    <td><audio controls="controls" type="audio/wav" src="/assets/icassp2020/samples/sample_5_398745627_five_gauss_8_ref.wav"><a>play</a></audio></td>
    <td><audio controls="controls" type="audio/wav" src="/assets/icassp2020/samples/sample_5_398745627_five_gauss_8_mix.wav"><a>play</a></audio></td>
    <td><audio controls="controls" type="audio/wav" src="/assets/icassp2020/samples/sample_5_398745627_five_gauss_8_source0.wav"><a>play</a></audio></td>
    <td>12.44 dB</td>
    <td>21.82 dB</td>
    <td>3</td>
    <td>0.747 s</td>
  </tr>
  <tr>
    <td>8</td>
    <td>2</td>
    <td>OverIVA</td>
    <td><audio controls="controls" type="audio/wav" src="/assets/icassp2020/samples/sample_5_398745627_overiva_gauss_8_ref.wav"><a>play</a></audio></td>
    <td><audio controls="controls" type="audio/wav" src="/assets/icassp2020/samples/sample_5_398745627_overiva_gauss_8_mix.wav"><a>play</a></audio></td>
    <td><audio controls="controls" type="audio/wav" src="/assets/icassp2020/samples/sample_5_398745627_overiva_gauss_8_source0.wav"><a>play</a></audio></td>
    <td>12.51 dB</td>
    <td>23.40 dB</td>
    <td>10</td>
    <td>1.129 s</td>
  </tr>
  <tr>
    <td>8</td>
    <td>2</td>
    <td>AuxIVA</td>
    <td><audio controls="controls" type="audio/wav" src="/assets/icassp2020/samples/sample_5_398745627_auxiva_gauss_8_ref.wav"><a>play</a></audio></td>
    <td><audio controls="controls" type="audio/wav" src="/assets/icassp2020/samples/sample_5_398745627_auxiva_gauss_8_mix.wav"><a>play</a></audio></td>
    <td><audio controls="controls" type="audio/wav" src="/assets/icassp2020/samples/sample_5_398745627_auxiva_gauss_8_source0.wav"><a>play</a></audio></td>
    <td>10.48 dB</td>
    <td>23.61 dB</td>
    <td>50</td>
    <td>22.919 s</td>
  </tr>
  <tr>
    <td>8</td>
    <td>3</td>
    <td>FIVE</td>
    <td><audio controls="controls" type="audio/wav" src="/assets/icassp2020/samples/sample_5_58984517_five_gauss_8_ref.wav"><a>play</a></audio></td>
    <td><audio controls="controls" type="audio/wav" src="/assets/icassp2020/samples/sample_5_58984517_five_gauss_8_mix.wav"><a>play</a></audio></td>
    <td><audio controls="controls" type="audio/wav" src="/assets/icassp2020/samples/sample_5_58984517_five_gauss_8_source0.wav"><a>play</a></audio></td>
    <td>14.03 dB</td>
    <td>21.15 dB</td>
    <td>3</td>
    <td>0.655 s</td>
  </tr>
  <tr>
    <td>8</td>
    <td>3</td>
    <td>OverIVA</td>
    <td><audio controls="controls" type="audio/wav" src="/assets/icassp2020/samples/sample_5_58984517_overiva_gauss_8_ref.wav"><a>play</a></audio></td>
    <td><audio controls="controls" type="audio/wav" src="/assets/icassp2020/samples/sample_5_58984517_overiva_gauss_8_mix.wav"><a>play</a></audio></td>
    <td><audio controls="controls" type="audio/wav" src="/assets/icassp2020/samples/sample_5_58984517_overiva_gauss_8_source0.wav"><a>play</a></audio></td>
    <td>14.26 dB</td>
    <td>21.88 dB</td>
    <td>10</td>
    <td>0.937 s</td>
  </tr>
  <tr>
    <td>8</td>
    <td>3</td>
    <td>AuxIVA</td>
    <td><audio controls="controls" type="audio/wav" src="/assets/icassp2020/samples/sample_5_58984517_auxiva_gauss_8_ref.wav"><a>play</a></audio></td>
    <td><audio controls="controls" type="audio/wav" src="/assets/icassp2020/samples/sample_5_58984517_auxiva_gauss_8_mix.wav"><a>play</a></audio></td>
    <td><audio controls="controls" type="audio/wav" src="/assets/icassp2020/samples/sample_5_58984517_auxiva_gauss_8_source0.wav"><a>play</a></audio></td>
    <td>13.33 dB</td>
    <td>20.47 dB</td>
    <td>50</td>
    <td>23.327 s</td>
  </tr>
</table>
