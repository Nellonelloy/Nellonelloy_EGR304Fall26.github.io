---
title: Component Selection
---

## Examples

### Style 1



*Table 1: component selection*

**Op-Amp**

| **Solution**                                                                                                                                                                                      | **Pros**                                                                                                                                    | **Cons**                                                                                            |
| ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | ------------------------------------------------------------------------------------------------------------------------------------------- | --------------------------------------------------------------------------------------------------- |
|<img src="https://github.com/user-attachments/assets/fb22a085-ec0a-428a-b031-995551954a36" width="64" height="64" alt="image" /> <br>Option 1.<br> TLV2464CN Operational Amplifier<br>$4.50/each<br>[link to product](https://www.digikey.com/en/products/detail/texas-instruments/TLV2464CN/374292)                 | \* Very low input offset<br>\* Low current input bias<br>\* Meets surface mount constraint of project                                               | \* Much more expensive than other options<br>\* Low operating temperature<br>\* Voltage supply minimum fairly high |
|<img width="64" height="64" alt="image" src="https://github.com/user-attachments/assets/4fa9080c-1607-4cdb-bb7e-7f2202e04139" /><br>\* Option 2. <br>\* TL974IN Operational Amplifier<br>\* $1.66/each <br>\* [Link to product](https://www.digikey.com/en/products/detail/texas-instruments/TL974IN/1675406) | \* Very good voltage supply max <br>\* Stable over operating temperature <br> \* Good voltage input offset | * Very bad current input bias <br>\* Bad Slew rate (not very important in my utilization)                                                         |
|<img width="72" height="72" alt="image" src="https://github.com/user-attachments/assets/c3adcd19-5112-49c0-b658-1be537a325ad" /> <br>Option 3.<br> MCP6004-I/P Operational Amplifier<br>$0.60/each<br>[link to product](https://www.digikey.com/en/products/detail/microchip-technology/MCP6004-I-P/523060)                 | \* Very low cheap<br>\* very good current input bias<br>\* Good voltage supply minimum                                               | \* Bad voltage input offset<br>\* Bad current output (not very important for my application) |
**Choice:** Option 3: the MCP6004-I/P Operational Amplifier

**Rationale:**  Available, low cost, and good input bias. It more than meets all of my requirements.

**Voltage Regulator**

| **Solution**                                                                                                                                                                                      | **Pros**                                                                                                                                    | **Cons**                                                                                            |
| ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | ------------------------------------------------------------------------------------------------------------------------------------------- | --------------------------------------------------------------------------------------------------- |
|<img width="200" height="200" alt="image" src="https://github.com/user-attachments/assets/3dac3cf1-8676-4492-bcf7-6819597ffdb7"/> <br>Option 1.<br> L7805ABV-DG Voltage Regulator<br>$1.53/each<br>[link to product](https://www.digikey.com/en/products/detail/stmicroelectronics/L7805ABV-DG/3945936) | \* Through Hole like other componenets<br>\* High current output<br>\* Meets surface mount constraint of project                                               | \* Much higher voltage dropout<br>\* More expensive<br>\* Less protection features |
|<img width="64" height="64" alt="image" src="https://github.com/user-attachments/assets/8899bc92-e759-4ab7-855c-9b756e20466b" /><br>\* Option 2. <br>\* AP7583Q-50D4-13 Voltage Regulator<br>\* $0.95/each <br>\* [Link to product](https://www.digikey.com/en/products/detail/diodes-incorporated/AP7583Q-50D4-13/22158461) | \*Low cost <br>\* Low voltage dropout <br> \* Fixed 5V output | * Surface mount and not through hole <br>\*Four prong instead of three (very unimportant other than increasing mounting time)|
|<img width="64" height="64" alt="image" src="https://github.com/user-attachments/assets/8d3177a0-d1fe-4be5-a39d-12a45ec5080a" /><br> Option 3.<br> AP7583AQ-50D4-13 Voltage Regulator<br>$1.01/each<br>[link to product](https://www.digikey.com/en/products/detail/diodes-incorporated/AP7583AQ-50D4-13/21823695)  | \* Cheap<br>\* 5V fixed ouput<br>\* Multiple control features | \* Not through hole<br>\* Four prong instead of three (very unimportant other than increasing mounting time)|
**Choice:** Option 1: L7805ABV-DG Voltage Regulator

**Rationale:** The voltage regulator I chose is a bit more expensive, but it's footprint is more compatible with my PCB than the others, and the advantages the other voltage regulators have over this one are of negligible difference for the purpose of this project.

**Pressure Sensor**

| **Solution**                                                                                                                                                                                      | **Pros**                                                                                                                                    | **Cons**                                                                                            |
| ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | ------------------------------------------------------------------------------------------------------------------------------------------- | --------------------------------------------------------------------------------------------------- |
|<img width="64" height="64" alt="image" src="https://github.com/user-attachments/assets/b6941021-2d8a-4149-accb-9c96164d94fa" /><br>Option 1.<br> CFSensor XGZP6878A15115KPA Pressure Sensor<br>$7.20/each<br>[link to product](https://www.digikey.com/en/products/detail/cfsensor/XGZP6878A15115KPA/22530803) | \* Cheap<br>\* Pressure range covers needed levels<br> | \* 2.5% margin of error worse than original requirements<br>\* Already amplified making op amp unecessary |
|<img width="64" height="64" alt="image" src="https://github.com/user-attachments/assets/86e7d69c-6a14-4767-bd57-fad963650086" /><br>Option 2.<br> Honeywell Sensing and Productivity Solutions 13U1000PA0K Pressure Sensor<br> $363.96/each <br> [Link to product](https://www.digikey.com/en/products/detail/honeywell-sensing-and-productivity-solutions/13U1000PA0K/10465927) | \*Accuracy within project bounds <br>\* Compatible with 5V power rail <br> \* Allows use of chosen op amp | * Extremely expensive <br>\*Out of stock at the supplier|
|<img width="64" height="64" alt="image" src="https://github.com/user-attachments/assets/1fd17e77-2a73-47be-83c2-e4980184f7e4" /><br> Option 3.<br> WEC 13U0500PA0K pressure sensor<br>$195.18/each<br>[link to product](https://www.digikey.com/en/products/detail/wec/13U0500PA0K/27528758)  | \* Allows use of op-amp<br>\* 0.25% margin of error<br>\* Compatible with 5v power rail | \* Extremely expensive<br>\* Large metal package |
**Choice:** Option 1:  CFSensor XGZP6878A15115KPA Pressure Sensor

**Rationale:** It is the only affordable option that was available that was also in stock.

**Power-Supply**

| **Solution**                                                                                                                                                                                      | **Pros**                                                                                                                                    | **Cons**                                                                                            |
| ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | ------------------------------------------------------------------------------------------------------------------------------------------- | --------------------------------------------------------------------------------------------------- |
|<img width="64" height="64" alt="image" src="https://github.com/user-attachments/assets/2f8be27e-cad6-4d5a-8d1c-1ca2255e1359" /><br>Option 1.<br> YINGJIAO YS6V-0900500-D1M power supply<br>$7.64/each<br>[link to product](https://www.digikey.com/en/products/detail/jameco-electronics/YS6V-0900500-D1M/25966413) | \* Cheap<br>\* Large onput voltage range<br>\*Compact| \* Low maximum output current<br>\* Minimum order quanitity of 2  |
|<img width="64" height="64" alt="image" src="https://github.com/user-attachments/assets/ad905b2f-cd44-4402-a15b-f8b11393c8d9" /><br>\* Option 2. <br>\* Pololu 1470 power supply<br>\* $11.41/each <br>\* [Link to product](https://www.digikey.com/en/products/detail/pololu/1470/19200211) | \* High current ouput <br>\* Regulated 9V output <br> \* Wide input voltage range | * Moderately expensive <br>\* Shorter power cord                                                         |
|<img width="64" height="64" alt="image" src="https://github.com/user-attachments/assets/84596c49-bff1-4f00-bb8e-9d9df76e0d54" /><br>Option 3.<br>Jameco ReliaPro GPU410900500WD00 Power Supply<br>$13.24/each<br>[link to product](https://www.digikey.com/en/products/detail/jameco-electronics/GPU410900500WD00/25966178) | \* Linear design<br>\* Regulated 9V output<br>\*Multiple safety approvals | \* Expensive<br>\* Only accepts 120V AC input |
**Choice:** Option 2:  Pololu 1470 Power Supply

**Rationale:** The power supply I chose has a regulated 9V output, high current capacity, and compatibility with my voltage regulator. The 1A output will be useful if there are any future modifications to the design.

## Pin Table

The following table identifies the pin connections used by the
PIC18F57Q43 Curiosity Nano in the pressure-sensing subsystem.

| PIC Pin | Function | Connected Component | Purpose |
|---|---|---|---|
| RA0 (ANA0) | Analog Input | CFSensor XGZP6878A15115KPA | Receives analog pressure measurements |
| RC2 (UART1 TX) | Serial Output | Team Communication Connector | Transmits pressure measurements |
| RC3 (UART1 RX) | Serial Input | Team Communication Connector | Receives communication from other subsystems |
| VTG | Power Input | L7805ABV-DG Voltage Regulator | Receives regulated 5V |
| GND | Ground | Common Ground | Provides ground reference |

### Pin Selection Rationale

The RA0 pin was selected because it supports analog-to-digital
conversion, allowing the PIC18F57Q43 to measure the analog voltage
produced by the pressure sensor without requiring an external
operational amplifier.

RC2 and RC3 were selected for UART communication between
subsystems. These assignments are preliminary and will be
confirmed when the team finalizes its communication interface.

The VTG and GND connections provide the microcontroller with
regulated 5V power from the L7805ABV-DG voltage regulator.
