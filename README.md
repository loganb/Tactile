Tactile
=============

Introduction
-------------

Tactile is a electic haptics device designed to provide computer-controlled sensory input. The power board contains 10x10 grid of pins designed to be pressed against the skin. Via a 20-pin ribbon cable, each pin may be independently activated to apply a gentle but detectable electric shock. Through this technique, it is possible to project a 100 pixel "image" onto the surface of the skin. 


WARNING
-------------

This design is untested and may be dangerous! Don't build it, don't use it, don't think about it unless you know what you're doing, know what the risks are, and know how to avoid them! 

Using
------------

The tactile board is connected to a microcontroller via a 20-pin connector. Each row (Y) and column (X) is controlled by one pin, active-low. Additionally, there is a 2-pin power connector to supply -100V and +5V. The row/column pins are active low. When one of each is shorted to ground, the pin at the insection swings from floating to -100V. A ground pad must contact the user's body at another location to form a complete circuit. 

Varying levels of sensation can be created through the use of PWM on the column lines. 

TODO
-------------

* Only the power board is currently designed, a companion board with a microcontroller and Voltage generation circuitry is TBD
* Board has yet to be fabricated, it may not work
* 100V may not be enough to form a reliable sensation

