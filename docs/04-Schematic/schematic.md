# Schematic

## Overview

This schematic illustrates the electrical design of my
pressure-sensing subsystem for the EGR 304 environmental
monitoring project.

The circuit incorporates a PIC18F57Q43 microcontroller,
an XGZP6887A pressure sensor, an MCP6004 operational
amplifier, and a 5V voltage regulator.

Additional components include a low-pass RC filter
for signal conditioning, a fuse for overcurrent
protection, and an 8-pin ribbon cable connector
for communication between subsystems.

The pressure sensor produces an analog voltage
corresponding to the measured pressure. The signal
is conditioned before being processed by the
PIC18F57Q43 microcontroller.

## Schematic

<img width="2445" height="1680" alt="image" src="https://github.com/user-attachments/assets/0497d139-c314-4e0d-a9e7-9b561a600dd1" />





**Figure 1:** Electrical schematic of the pressure-sensing
subsystem.

## Resources

The complete electrical schematic is available below.

[Download Schematic PDF](EGR-304_Pressure-Sensor.pdf)

[Download KiCad Project ZIP](EGR_304_Schematic_First_Updated_Nov09.zip)
