This is a port to Energia of the famous LedControl arduino library
-------------------------------------------------------------------

Originally written for Arduino and MAX7219, this library works with minor changes with
MSP430 Energia and AS1106 or AS1107.

AS1106 or AS1107 are MAX7219 or MAX7221 clones made by AMS chip maker, these devices work from 2.7 to 5.5 V
while the MAX7219 officially work only at 5 V (while I succesfully tested them at 3.3 V).

The examples folder contains the original examples (changed to the new API but untested) and an additional MSP430 example
(tested on Launchpad with MSP430G2553).

The main difference from the original library is that you need to call LedControl::init() in your setup, the initialization which
was originally done in the constructor did not work with MSP430.

Enjoy!