---
title: CompactSix Microphone Array
layout: project
tagline: "A compact array with 6 channels."
description: "Built with a Beaglebone Black at its core, this array packs some punch for practical implementations and demos."
klass: hardware
images: images/compactsix.png
links:
  - icon: github
    url: https://github.com/LCAV/CompactSix
hidden: true
---

The CompactSix array project was started in the summer of 2014 when I decided I needed a platform
to conduct practical experiments for multichannel processing algorithms. My initial design was
a cape for the Beaglebone Black sporting a six channels PDM microphone processor chip (STA321MP).
After a lot of struggle, I managed to write the ALSA driver for this processor...
Only to discover about a year later that the STA321MP was not supported anymore when I asked the manufacturer
for help with some of the functionalities.

Frustrated by this and also due to the lack of real-time capability of the ALSA framework, I
decided to do all the PDM decoding in one of the programmable realtime units (PRU) of the BBB.
I was very lucky then to receive the help of Loïc Droz who did the implementation of the CIC
filters in the PRU. I produced then a new hardware design for possible 8 channels (only 6 supported
in processing now). The new hardware design allows both for keeping the array all on one PCB, or
cutting off the microphnes and using wires for more flexible geometries.
