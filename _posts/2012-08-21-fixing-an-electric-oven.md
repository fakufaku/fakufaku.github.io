---
layout: post
title: "Fixing an Electric Oven"
description: "Electric oven convesion using Arduino"
tagline: "Coming soon: cakes!"
category: hacks
tags: [hack, oven, TokyoTime]
---
{% include JB/setup %}

I recently received from a friend an abandoned oven. My friend had partially fixed it using a massive AC relay to switch the heating element on and off using a 5V DC relay itself switched by an arduino.

When I received it however, only the big AC relay was left. Proper temperature control had also never been implemented, despite a thermistor being present in the oven.

I also had at hand the [TokyoTime](https://github.com/fakufaku/TokyoTime), an
Arduino based 7-segment clock based on a
[SparkFun](https://www.sparkfun.com/products/10870)
[design](https://github.com/sparkfun/BigTime).  Using the TokyoTime has two
advantages. I have a display right away, and buttons, and 5V power supply, and
I have exactly two free pins, analog ones. I can thus use one to read the
thermistor providing the temperature inside the oven, and use the other to
switch the relay on and off.  The TokyoTime runs at 3.3V, I use a common
wall-wart switching supply to transform the 110 AC into 5V DC. For convenience,
I have added a female plug inside the oven.

![Guts of the oven]({{ site.url }}/resource/photos/oven/oven2.jpg)

Since the 5V DC relay draws too much current to be driven from a pin directly, we need a MOSFET transistor driver. The following diagram gives an idea of the driving circuit.

![Diagram]({{ site.url }}/resource/photos/oven/oven3.jpg) ![Driver circuit]({{ site.url }}/resource/photos/oven/oven1.jpg)

For the temperature control, I use the arduino [PID
Library](http://arduino.cc/playground/Code/PIDLibrary). Using trial and error,
I settled on PID constants, probably not perfect but converging to the set
point temperature after some time. I use the button on the TokyoTime to set the
desired temperature of the oven. Setting the temperature to zero effectively
shut down the heating. However, it still needs to be unplugged to be totally
off.  The firmware used for the TokyoTime board (codenamed 'Kuishimbo') can be
found in this [repo](https://github.com/fakufaku/Kuishimbo).

Finally, I neatly arranged the driver circuit in a Tupperware box and glued the TokyoTime on the outside of the oven where the old display was.

![Inside]({{ site.url }}/resource/photos/oven/oven4.jpg) ![Outside]({{ site.url }}/resource/photos/oven/oven5.jpg)

