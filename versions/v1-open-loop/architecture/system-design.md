# Open Loop System Architecture

This document outlines the core hardware blocks of the open-loop inverter.

## Block Diagram Overview
1. **Microcontroller:** Generates the SPWM signals.
2. **Gate Driver:** Steps up the logic-level SPWM to adequately drive the MOSFET gates.
3. **H-Bridge Inverter:** Switches the 12V DC across the transformer primary.
4. **Step-Up Transformer:** Converts the switched 12V AC to 230V AC.

## Circuit Sub-Systems
* **SPWM Generation:** [Insert details about your microcontroller setup]
* **Power Stage:** Utilizing the IR2104 half-bridge drivers to control the IRFZ44N MOSFETs.

*(Upload schematic images to the `/media` folder and link them here later)*
