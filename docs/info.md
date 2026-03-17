<!---

This file is used to generate your project datasheet. Please fill in the information below and delete any unused
sections.

You can also include images in this folder and reference them in the markdown. Each image must be less than
512 kb in size, and the combined size of all images must be less than 1 MB.
-->

## How it works

The design targets two ring oscillators operating at approximately 600 MHz and 300 MHz. Due to pad loading, the output signal is expected to be attenuated. 
The first oscillator consists of 18 inverters along with a NAND gate for enable control, 
while the second oscillator uses 36 inverters and a NAND gate. To ensure sufficient output drive strength, a two-stage inverter buffer with large-sized transistors is employed.

## How to test

Enable 600 MHz oscillator 1 by setting user input pin 0 high and measure the signal at analog output 0.
Enable 300 MHz oscillator 2 by setting user input pin 1 high and measure the signal at analog output 1.
The 300 MHz ring oscillator had a problem with a missing contact in TT08, and is not expected to work. It has been fixed for TT09.

## External hardware

Oscilloscope.
