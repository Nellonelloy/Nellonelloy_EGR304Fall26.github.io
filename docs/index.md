---
title: Welcome
tags:
- tag1
- tag2
---
<center>
<font size= "6"> Brendan Datasheet</font><br>
as part of<br>
<font size= "8"> Weather Reader</font><br>
for<br>
<font size= "5"> Team 202 </font><br>

**Submission: 10/30/2026
</center>

## Introduction

* My name is Brendan, an Electrical Systems Engineering student at ASU, and this will be a data sheet to showcase and record my individual efforts to the creation of the weather device outside of just the team specific work. 
### Project Summary

Our EGR 304 team project involves designing and developing an environmental monitoring system capable of measuring atmospheric pressure, temperature, humidity, and light levels. My individual contribution focuses on designing a PCB that uses a pressure sensor, operational amplifier, low-pass filter, and PIC18F57Q43 microcontroller to accurately measure and process atmospheric pressure data. This subsystem will communicate with the team's other PCBs through UART, allowing the collected measurements to be displayed on a central LCD screen and contributing to the overall functionality of the environmental monitoring system.

* Add context that ties into the link to your [team report.](https://embedded-systems-design.github.io/EGR304TeamTemplate/)


### My Contribution

My contribution to the weather sensing device is the pressure sensor. It reads absolute pressure as an analog signal, converts it into a readable digital signal, and sends it to my teammates PCB.

To review the details listed of the material used to construct the subsection, you can review it in the ["BOM"](https://embedded-systems-design.github.io/EGR304DataSheetTemplate/03-BOM/BOM/) section of the datasheet.

For all the sections
## Project Documentation

The following sections document the design and development
of my pressure-sensing subsystem.

### Component Selection

This section compares potential components for the
pressure-sensing subsystem, including the pressure sensor,
voltage regulator, and power supply.

[View Component Selection](02-Component-Selection/Component-Selection.md)

### Power Budget

This section provides the estimated power consumption
of the subsystem and verifies that the selected
power supply and voltage regulator can provide
sufficient current.

[View Power Budget](05-Power-Budget/Power-Budget.md)

### Schematic

This section presents the electrical schematic for my
pressure-sensing subsystem. The design includes a
PIC18F57Q43 microcontroller, pressure sensor,
voltage regulator, operational amplifier,
low-pass filter, and ribbon cable connector.

[View Schematic](04-Schematic/EGR_304_Schematic_First.pdf)
