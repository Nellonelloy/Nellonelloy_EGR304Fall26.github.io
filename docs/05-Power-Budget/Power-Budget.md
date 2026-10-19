---
title: Power Budget
---

## Overview

The purpose of this power budget is to determine the electrical power requirements of my pressure-sensing subsystem and ensure that the selected voltage regulator and external power supply can safely operate all components.

The subsystem uses a Pololu 1470 power supply to provide 9V DC to an L7805ABV-DG voltage regulator, which converts the voltage to 5V. This regulated 5V supply powers the PIC18F57Q43 Curiosity Nano and the CFSensor XGZP6878A15115KPA pressure sensor.

The total estimated current consumption of the components was calculated, and a 25% safety margin was added to account for potential variations in power consumption.

## Power Budget

The power budget was divided into four sections:

- Section A: Maximum current consumption of major components.
- Section B: Power rail assignments and safety margin.
- Section C: Voltage regulator selection and available current.
- Section D: External power supply selection and available current.

The system operates using a single regulated 5V power rail.

### Power Budget Summary

| Component | Estimated Current |
|---|---|
| PIC18F57Q43 Curiosity Nano | 20 mA |
| CFSensor XGZP6878A15115KPA | 5 mA |
| Curiosity Nano Support Circuitry | 0.005 mA |
| Total Current | 25.005 mA |
| 25% Safety Margin | 6.251 mA |
| Total Required Current | 31.256 mA |

The PIC and pressure sensor current values are provisional estimates and will require verification against manufacturer specifications or physical testing.

### Power Budget Calculations

![Power Budget Section 1](PressureBudget1.png)

![Power Budget Section 2](PressureBudget2.png)

![Power Budget Section 3](PressureBudget3.png)

## Conclusions

The power budget indicates that the selected power supply and voltage regulator have sufficient current capacity to operate the pressure-sensing subsystem.

The estimated total current requirement is 31.256 mA after including the 25% safety margin.

The L7805ABV-DG voltage regulator is rated to supply up to 1500 mA, which exceeds the subsystem's estimated requirements.

The Pololu 1470 power supply provides 9V at a maximum of 1000 mA. Including a provisional 8 mA allowance for regulator current consumption, the estimated input current requirement is 39.256 mA. This leaves approximately 960.744 mA of available current capacity.

These calculations suggest that the selected components are suitable for the subsystem's power requirements. However, the maximum current consumption of the microcontroller, pressure sensor, and voltage regulator should be verified before the final design review.

## Resources

The completed power budget is available in the following formats:

- [Power Budget PDF](PressurePowerBudget.pdf)
- [Power Budget Excel Spreadsheet](PressurePowerBudget.xlsx)
