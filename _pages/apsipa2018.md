---
title: "APSIPA 2018"
layout: project
tagline: "Blinkies: Sound-to-light conversion sensors and their application to speech enhancement and sound source localization"
description: "We use distributed devices converting sound to light and acquire the signals using a camera."
permalink: /apsipa2018
klass: audio
images: images/blinky.png
hidden: true
---

## Abstract

We introduce the use of blinkies for acoustic sensing and audio processing
applications. Blinkies are low-power sensors with a microphone and an LED that
can be easily distributed over a large area. The power of the LED is modulated
by the sound intensity and the signals from all devices can be captured by a
regular video camera. We present our design for blinkies and characterize the
transmission function from blinky to captured video signal. The usefulness of
such a system is demonstrated with two applications. First, we evaluate
beamforming informed by a high-quality voice activity signal obtained from a
blinky. Second, we investigate sound source localization using several blinkies
distributed in a room.

## Audio Samples

<style type="text/css">
audio {
width: 50px;
}
</style>

<table>
<tr>
<td>SIR</td>
<td>Target</td>
<td>Mix</td>
<td colspan="2">AuxIVA</td>
<td colspan="2">Max-SINR</td>
</tr>

<tr>
<td></td>
<td></td>
<td></td>
<td>2 ch</td>
<td>4 ch</td>
<td>2 ch</td>
<td>4 ch</td>
<td>24 ch</td>
<td>48 ch</td>
</tr>
<tr>
<td>-5</td>
<td><audio controls="controls" type="audio/wav" src="/assets/apsipa2018/samples/pyramic_2_ref_SIR_NA_dB.wav"><a>play</a></audio></td>
<td><audio controls="controls" type="audio/wav" src="/assets/apsipa2018/samples/pyramic_2_mix_SIR_-5_dB.wav"><a>play</a></audio></td>
<td><audio controls="controls" type="audio/wav" src="/assets/apsipa2018/samples/pyramic_2_bss_SIR_-5_dB.wav"><a>play</a></audio></td>
<td><audio controls="controls" type="audio/wav" src="/assets/apsipa2018/samples/pyramic_4_bss_SIR_-5_dB.wav"><a>play</a></audio></td>
<td><audio controls="controls" type="audio/wav" src="/assets/apsipa2018/samples/pyramic_2_maxsinr_SIR_-5_dB.wav"><a>play</a></audio></td>
<td><audio controls="controls" type="audio/wav" src="/assets/apsipa2018/samples/pyramic_4_maxsinr_SIR_-5_dB.wav"><a>play</a></audio></td>
<td><audio controls="controls" type="audio/wav" src="/assets/apsipa2018/samples/pyramic_24_maxsinr_SIR_-5_dB.wav"><a>play</a></audio></td>
<td><audio controls="controls" type="audio/wav" src="/assets/apsipa2018/samples/pyramic_48_maxsinr_SIR_-5_dB.wav"><a>play</a></audio></td>
</tr>
<tr>
<td>0</td>
<td><audio controls="controls" type="audio/wav" src="/assets/apsipa2018/samples/pyramic_2_ref_SIR_NA_dB.wav"><a>play</a></audio></td>
<td><audio controls="controls" type="audio/wav" src="/assets/apsipa2018/samples/pyramic_2_mix_SIR_0_dB.wav"><a>play</a></audio></td>
<td><audio controls="controls" type="audio/wav" src="/assets/apsipa2018/samples/pyramic_2_bss_SIR_0_dB.wav"><a>play</a></audio></td>
<td><audio controls="controls" type="audio/wav" src="/assets/apsipa2018/samples/pyramic_4_bss_SIR_0_dB.wav"><a>play</a></audio></td>
<td><audio controls="controls" type="audio/wav" src="/assets/apsipa2018/samples/pyramic_2_maxsinr_SIR_0_dB.wav"><a>play</a></audio></td>
<td><audio controls="controls" type="audio/wav" src="/assets/apsipa2018/samples/pyramic_4_maxsinr_SIR_0_dB.wav"><a>play</a></audio></td>
<td><audio controls="controls" type="audio/wav" src="/assets/apsipa2018/samples/pyramic_24_maxsinr_SIR_0_dB.wav"><a>play</a></audio></td>
<td><audio controls="controls" type="audio/wav" src="/assets/apsipa2018/samples/pyramic_48_maxsinr_SIR_0_dB.wav"><a>play</a></audio></td>
</tr>
<tr>
<td>5</td>
<td><audio controls="controls" type="audio/wav" src="/assets/apsipa2018/samples/pyramic_2_ref_SIR_NA_dB.wav"><a>play</a></audio></td>
<td><audio controls="controls" type="audio/wav" src="/assets/apsipa2018/samples/pyramic_2_mix_SIR_5_dB.wav"><a>play</a></audio></td>
<td><audio controls="controls" type="audio/wav" src="/assets/apsipa2018/samples/pyramic_2_bss_SIR_5_dB.wav"><a>play</a></audio></td>
<td><audio controls="controls" type="audio/wav" src="/assets/apsipa2018/samples/pyramic_4_bss_SIR_5_dB.wav"><a>play</a></audio></td>
<td><audio controls="controls" type="audio/wav" src="/assets/apsipa2018/samples/pyramic_2_maxsinr_SIR_5_dB.wav"><a>play</a></audio></td>
<td><audio controls="controls" type="audio/wav" src="/assets/apsipa2018/samples/pyramic_4_maxsinr_SIR_5_dB.wav"><a>play</a></audio></td>
<td><audio controls="controls" type="audio/wav" src="/assets/apsipa2018/samples/pyramic_24_maxsinr_SIR_5_dB.wav"><a>play</a></audio></td>
<td><audio controls="controls" type="audio/wav" src="/assets/apsipa2018/samples/pyramic_48_maxsinr_SIR_5_dB.wav"><a>play</a></audio></td>
</tr>
<tr>
<td>10</td>
<td><audio controls="controls" type="audio/wav" src="/assets/apsipa2018/samples/pyramic_2_ref_SIR_NA_dB.wav"><a>play</a></audio></td>
<td><audio controls="controls" type="audio/wav" src="/assets/apsipa2018/samples/pyramic_2_mix_SIR_10_dB.wav"><a>play</a></audio></td>
<td><audio controls="controls" type="audio/wav" src="/assets/apsipa2018/samples/pyramic_2_bss_SIR_10_dB.wav"><a>play</a></audio></td>
<td><audio controls="controls" type="audio/wav" src="/assets/apsipa2018/samples/pyramic_4_bss_SIR_10_dB.wav"><a>play</a></audio></td>
<td><audio controls="controls" type="audio/wav" src="/assets/apsipa2018/samples/pyramic_2_maxsinr_SIR_10_dB.wav"><a>play</a></audio></td>
<td><audio controls="controls" type="audio/wav" src="/assets/apsipa2018/samples/pyramic_4_maxsinr_SIR_10_dB.wav"><a>play</a></audio></td>
<td><audio controls="controls" type="audio/wav" src="/assets/apsipa2018/samples/pyramic_24_maxsinr_SIR_10_dB.wav"><a>play</a></audio></td>
<td><audio controls="controls" type="audio/wav" src="/assets/apsipa2018/samples/pyramic_48_maxsinr_SIR_10_dB.wav"><a>play</a></audio></td>
</tr>
<tr>
<td>15</td>
<td><audio controls="controls" type="audio/wav" src="/assets/apsipa2018/samples/pyramic_2_ref_SIR_NA_dB.wav"><a>play</a></audio></td>
<td><audio controls="controls" type="audio/wav" src="/assets/apsipa2018/samples/pyramic_2_mix_SIR_15_dB.wav"><a>play</a></audio></td>
<td><audio controls="controls" type="audio/wav" src="/assets/apsipa2018/samples/pyramic_2_bss_SIR_15_dB.wav"><a>play</a></audio></td>
<td><audio controls="controls" type="audio/wav" src="/assets/apsipa2018/samples/pyramic_4_bss_SIR_15_dB.wav"><a>play</a></audio></td>
<td><audio controls="controls" type="audio/wav" src="/assets/apsipa2018/samples/pyramic_2_maxsinr_SIR_15_dB.wav"><a>play</a></audio></td>
<td><audio controls="controls" type="audio/wav" src="/assets/apsipa2018/samples/pyramic_4_maxsinr_SIR_15_dB.wav"><a>play</a></audio></td>
<td><audio controls="controls" type="audio/wav" src="/assets/apsipa2018/samples/pyramic_24_maxsinr_SIR_15_dB.wav"><a>play</a></audio></td>
<td><audio controls="controls" type="audio/wav" src="/assets/apsipa2018/samples/pyramic_48_maxsinr_SIR_15_dB.wav"><a>play</a></audio></td>
</tr>
<tr>
<td>20</td>
<td><audio controls="controls" type="audio/wav" src="/assets/apsipa2018/samples/pyramic_2_ref_SIR_NA_dB.wav"><a>play</a></audio></td>
<td><audio controls="controls" type="audio/wav" src="/assets/apsipa2018/samples/pyramic_2_mix_SIR_20_dB.wav"><a>play</a></audio></td>
<td><audio controls="controls" type="audio/wav" src="/assets/apsipa2018/samples/pyramic_2_bss_SIR_20_dB.wav"><a>play</a></audio></td>
<td><audio controls="controls" type="audio/wav" src="/assets/apsipa2018/samples/pyramic_4_bss_SIR_20_dB.wav"><a>play</a></audio></td>
<td><audio controls="controls" type="audio/wav" src="/assets/apsipa2018/samples/pyramic_2_maxsinr_SIR_20_dB.wav"><a>play</a></audio></td>
<td><audio controls="controls" type="audio/wav" src="/assets/apsipa2018/samples/pyramic_4_maxsinr_SIR_20_dB.wav"><a>play</a></audio></td>
<td><audio controls="controls" type="audio/wav" src="/assets/apsipa2018/samples/pyramic_24_maxsinr_SIR_20_dB.wav"><a>play</a></audio></td>
<td><audio controls="controls" type="audio/wav" src="/assets/apsipa2018/samples/pyramic_48_maxsinr_SIR_20_dB.wav"><a>play</a></audio></td>
</tr>

</table>
