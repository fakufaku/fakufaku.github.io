---
layout: post
title: "Otemba v1.0"
tagline: "Tokyo Hackerspace's Arduino Clone"
description: "An Arduino clone for breadboard prototyping, made in Japan."
image: otemba/Otemba_dice.jpg
---

A few weeks ago, we decided on the mailing list of the [Tokyo Hackerspace](http://www.tokyohackerspace.org) that we need an Arduino clone.
It is common at the beginning of a new project to use a full-blown Arduino but then to go with the bare Atmega328 chip for the final version for space, cost reasons.
And in such case my thinking was that it would be great to have a small PCB where you can create a minimal version of the Arduino platform, with some flexibility
regarding voltage, regulator and crystal frequency. And if everything could be through-hole and off-the-shelf our [local electronics wonderland](http://www.akizukidenshi.com/)
it would be perfect.

After lots of [discussions](https://groups.google.com/d/topic/tokyohackerspace/dlDaHFsToPs/discussion) and many great input from Marco (who suggested the breadboard type),
I started a design on Eagle with the following criteria:

* Small size (max 5x5cm so that it can be ordered at [Seeed Studio](http://www.seeedstudio.com/) for the lowest price),

* All 20 I/O pins on one side, pluggable to breadboard,

* Footprints for a power regulator (available in 5V or 3.3V),

* Footprints for a battery booster, that comes handy when working on off-the-grid projects,

* Usable at 5V/16MHz or 3.3V/8MHz, by picking up the right components.

The result is the _Otemba_ v1.0. Otemba means 'tomboy' in Japanese and was chosen because the board is boyish, but still small and cute. Eagle designe files can be found on [github](https://github.com/TokyoHackerspace/Otemba).

![Front]({{ site.baseurl}}/content/images/otemba/Otemba_top.png)
![Back]({{ site.baseurl}}/content/images/otemba/Otemba_bot.png)

To demonstrate the breadboarding and prototyping capabilities of the Otemba, I have created a simple digital dice using a 7-segment digit and an LED for added flashiness.

![Digital Dice]({{ site.baseurl }}/content/images/otemba/Otemba_dice.jpg)

The code is in the [Dice7Seg repo](https://github.com/TokyoHackerspace/Dice7Seg). It uses freewheeling Timer1 and sample about every 100ms to display a number between 1 and 6. There is also a tactile switch that will choose the number in the counter when pressed and display it blinking slowly. When the button is pressed again, the numbers start spinning again.
