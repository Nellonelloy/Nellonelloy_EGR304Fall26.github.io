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
**Choice:** Option 3:  MCP6004-I/P Operational Amplifier

**Rationale:** The Op-Amp I chose is cheap, and it has a low voltage minimum supply. The biggest weakness of this one is the voltage input offset, but since we are going for an update every 2 seconds this is a sacrifice that I feel will have negiligble inpact.

**Voltage Regulator**

| **Solution**                                                                                                                                                                                      | **Pros**                                                                                                                                    | **Cons**                                                                                            |
| ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | ------------------------------------------------------------------------------------------------------------------------------------------- | --------------------------------------------------------------------------------------------------- |
|<img width="200" height="200" alt="image" src="https://github.com/user-attachments/assets/3dac3cf1-8676-4492-bcf7-6819597ffdb7"/> <br>Option 1.<br> L7805ABV-DG Voltage Regulator<br>$1.53/each<br>[link to product](https://www.digikey.com/en/products/detail/stmicroelectronics/L7805ABV-DG/3945936) | \* Through Hole like other componenets<br>\* High current output<br>\* Meets surface mount constraint of project                                               | \* Much higher voltage dropout<br>\* More expensive<br>\* Less protection features |
|<img width="64" height="64" alt="image" src="https://github.com/user-attachments/assets/8899bc92-e759-4ab7-855c-9b756e20466b" /><br>\* Option 2. <br>\* AP7583Q-50D4-13 Voltage Regulator<br>\* $0.95/each <br>\* [Link to product](https://www.digikey.com/en/products/detail/diodes-incorporated/AP7583Q-50D4-13/22158461) | \*Low cost <br>\* Low voltage dropout <br> \* Fixed 5V output | * Surface mount and not through hole <br>\*Four prong instead of three (very unimportant other than increasing mounting time)|
|<img width="64" height="64" alt="image" src="https://github.com/user-attachments/assets/8d3177a0-d1fe-4be5-a39d-12a45ec5080a" /><br> Option 3.<br> AP7583AQ-50D4-13 Voltage Regulator<br>$1.01/each<br>[link to product](https://www.digikey.com/en/products/detail/diodes-incorporated/AP7583AQ-50D4-13/21823695)  | \* Cheap<br>\* 5V fixed ouput<br>\* Multiple control features | \* Not through hole<br>\* Four prong instead of three (very unimportant other than increasing mounting time)|
**Choice:** Option 1: L7805ABV-DG Voltage Regulator

**Rationale:** The voltage regulator I chose is a bit more expensive, but it's footprint is more compatible with my PCB than the others, and the advantages the other voltage regulators have over this one are of negligible difference for the purpose of this project.

**Photoresistor**

| **Solution**                                                                                                                                                                                      | **Pros**                                                                                                                                    | **Cons**                                                                                            |
| ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | ------------------------------------------------------------------------------------------------------------------------------------------- | --------------------------------------------------------------------------------------------------- |
|<img width="64" height="64" alt="image" src="https://github.com/user-attachments/assets/93635b16-25ce-420c-beb9-0c158fae6be9" /><br>Option 1.<br> NSL-5150 Photoresistor<br>$4.53/each<br>[link to product](https://www.digikey.com/en/products/detail/advanced-photonix/NSL-5150/5039798) | \* 550nm wavelength<br>\* Very high dark resistance<br>\* 10k-20k illuminance resistance | \* Expensive<br>\* Photoresistors lose accuracy in high light conditions |
|<img width="64" height="64" alt="image" src="https://github.com/user-attachments/assets/29229db8-cb9f-45cf-a306-8094746f768e" /><br>\* Option 2. <br>\* NSL-5152 Photoresistor<br>\* $0.96/each <br>\* [Link to product](https://www.digikey.com/en/products/detail/advanced-photonix/NSL-5152/5423680) | \*Low cost <br>\* 10k-20k illuminance resistance <br> \* 550nm wavelength | * Photoresistors have low accuracy in high sunlight <br>\*half the dark cell resistance|
|<img width="200" height="200" alt="image" src="https://github.com/user-attachments/assets/d1cdba6d-509e-4da7-8e05-09d5c09cfe68" /><br> Option 3.<br> NSL-A6011 Photoresistor<br>$0.88/each<br>[link to product](https://www.digikey.com/en/products/detail/advanced-photonix/NSL-A6011/26316778?s=N4IgTCBcDaIHIGUAyBaAggNgAwEYcgF0BfIA)  | \* Cheap<br>\* Documented gamma value<br>\* compact | \* A little outside the optimal wavelength range<br>\* Low dark resistance |
**Choice:** Option 3: NSL-A6011 Photoresistor

**Rationale:** Although the other two options beat out the A6011 in every category other than price, the fact that we have a documented gamma value gives us a reference point for our code, which will make our reading more accurate.

