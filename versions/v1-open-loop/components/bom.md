# Bill of Materials (BOM) & Datasheets

Below is the hardware list required for the open-loop inverter prototype.

## Core Components

| Component | Part Number / Specs | Quantity | Purpose |
| :--- | :--- | :--- | :--- |
| Microcontroller | [e.g., ESP32 / Arduino Uno] | 1 | SPWM Generation |
| Gate Driver | IR2104 | 2 | Drives the H-Bridge MOSFETs |
| MOSFETs | IRFZ44N | 4 | High-speed power switching |
| Transformer | 12-0-12V to 230V | 1 | Voltage step-up |
| Diodes | 1N4007 / UF4007 | 2 | Bootstrap diodes for IR2104 |
| Capacitors | 10uF, 0.1uF | Var | Bootstrap and decoupling |

## Reference Datasheets
*It is highly recommended to review the switching characteristics before testing.*
* [IR2104 Gate Driver Datasheet](https://www.infineon.com/dgdl/Infineon-IR2104-DS-v01_00-EN.pdf?fileId=5546d462533600a4015355c7c1c31671)
* [IRFZ44N MOSFET Datasheet](https://www.infineon.com/dgdl/Infineon-IRFZ44N-DataSheet-v01_01-EN.pdf?fileId=5546d462533600a40153563b3a9f220d)
