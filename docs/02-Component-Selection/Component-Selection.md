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

**Rationale:** A clock oscillator is easier to work with because it requires no external circuitry in order to interface with the PSoC. This is particularly important because we are not sure of the electrical characteristics of the PCB, which could affect the oscillation of a crystal. While the shipping speed is slow, according to the website if we order this week it will arrive within 3 weeks.

### Style 2

> Also acceptable, more markdown friendly

**External Clock Module**

1. XC1259TR-ND surface mount crystal

    ![](image1.png)

    * $1/each
    * [link to product](http://www.digikey.com/product-detail/en/ECS-40.3-S-5PX-TR/XC1259TR-ND/827366)

    | Pros                                      | Cons                                                             |
    | ----------------------------------------- | ---------------------------------------------------------------- |
    | Inexpensive                               | Requires external components and support circuitry for interface |
    | Compatible with PSoC                      | Needs special PCB layout.                                        |
    | Meets surface mount constraint of project |

1. CTX936TR-ND surface mount oscillator

    ![](image3.png)

    * $1/each
    * [Link to product](http://www.digikey.com/product-detail/en/636L3I001M84320/CTX936TR-ND/2292940)

    | Pros                                                              | Cons                |
    | ----------------------------------------------------------------- | ------------------- |
    | Outputs a square wave                                             | More expensive      |
    | Stable over operating temperature                                 | Slow shipping speed |
    | Direct interface with PSoC (no external circuitry required) range |

**Choice:** Option 2: CTX936TR-ND surface mount oscillator

**Rationale:** A clock oscillator is easier to work with because it requires no external circuitry in order to interface with the PSoC. This is particularly important because we are not sure of the electrical characteristics of the PCB, which could affect the oscillation of a crystal. While the shipping speed is slow, according to the website if we order this week it will arrive within 3 weeks.
