---
title: Microphone Arrays
layout: project
tagline: "MEMS Compact Microphone Arrays"
description: "I like to build microphone arrays. Now I have a small collection."
klass: hardware
permalink: /microphone_arrays
images: images/pyramic.png
links:
  - icon: github
    url: https://github.com/LCAV/Pyramic
hidden: true
---

Over the last few years, with the help of several people, (René Beuchat, Eric
Bezzam, Juan Azcarreta Ortiz, Corentin Ferry, and Loïc Droz), I have built
several microphone array systems that I currently regularly use for demos
and experiments.

### Pyramic

My flagship microphone array is the [Pyramic](https://github.com/LCAV/pyramic) 48 channels
microphone array. It has a flexible semi-reconfigurable configuration. It is constructed
of long and thin PCB each sporting 8 MEMS microphones and an AD converter. Two PCB can
Be daisy chained and in the end connect to an FPGA/ARM system.

The array was tested in an anechoic chamber and a large dataset of recordings
were done there. The dataset can be used to test direction of arrival
algorithms.

### Compact Six

<img src="/images/compactsix.png">

The [CompactSix](https://github.com/LCAV/compactsix) array project was started
in the summer of 2014 when I decided I needed a platform to conduct practical
experiments for multichannel processing algorithms. My initial design was a
cape for the Beaglebone Black sporting a six channels PDM microphone processor
chip (STA321MP).  After a lot of struggle, I managed to write the ALSA driver
for this processor...  Only to discover about a year later that the STA321MP
was not supported anymore when I asked the manufacturer for help with some of
the functionalities.

### Kurodako

Frustrated by this and also due to the lack of real-time capability of the ALSA
framework, I decided to do all the PDM decoding in one of the programmable
realtime units (PRU) of the BBB.  I was very lucky then to receive the help of
[Loïc Droz](https://github.com/Scrashdown) who did the implementation of the
CIC filters in the PRU. I produced then a [new hardware
design](https://github.com/fakufaku/kurodako) for possibly 8 channels (only 6
supported in processing now). The new hardware design allows both for keeping
the array all on one PCB, or cutting off the microphnes and using wires for
more flexible geometries.

### Easy DSP

[Easy DSP](https://github.com/LCAV/easy-dsp) is a system that lets us interact
in real time with the output from the microphone arrays.  It has two parts. One
is a small C daemon that runs on the embedded Linux onboard the microphone
array (CompactSix or Pyramic) and opens a Web Socket delivering the audio data
over the network.  The other part is a web based interface that can retrieve
the audio samples and start python snippet to process the audio. It can also
receive back some data to plot from the Python script.
