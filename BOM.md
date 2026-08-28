# Bill of Materials (BOM)

| Designator(s) | Qty | Value / Part Number | Description | Footprint (Typical) |
| :--- | :---: | :--- | :--- | :--- |
| **Integrated Circuits & Semiconductors** | | | | |
| U1 | 1 | **STM32F103C8T6** | ARM Cortex-M3 Microcontroller (72MHz) | LQFP-48 |
| U2 | 1 | **AMS1117-3.3V** | 1A Low Dropout (LDO) Voltage Regulator | SOT-223 |
| U3 | 1 | **ESD Protection** | USB Data Line ESD Protection Diode | SOT-23-6 / SOT-666 |
| D1 | 1 | **LED Green** | Power Indicator LED | 0805 SMD |
| **Crystals & Oscillators** | | | | |
| X1 | 1 | **8 MHz Crystal** | High-Speed External (HSE) Clock | ABM3 (5.0x3.2mm SMD) |
| X2 | 1 | **32.768 kHz Crystal**| Low-Speed External (LSE) RTC Clock | ABS25 SMD |
| **Connectors & Switches** | | | | |
| J1 | 1 | **USB Type-C** | 16-Pin / 24-Pin USB-C Receptacle | SMD + TH Shield |
| SW1, SW2 | 2 | **Push Button** | Tactile Switch (BOOT0 and NRST) | 4-Pin SMD / TH |
| J2, J3, J6, J7 | 4 | **4-Pin Header** | 4x4 Female Header (GPIO Breakout, UART, ST-Link, Power) | 2.54mm Pitch TH |
| J4, J5 | 2 | **10-Pin Header** | 2x10 Female Header (GPIO Breakout) | 2.54mm Pitch TH |
| **Resistors** | | | | |
| R4, R5 | 2 | **5.1 kΩ** | ±1% USB-C CC Pull-down Resistors | 0805 SMD |
| R6, R7 | 2 | **10 kΩ** | ±1% Pull-up / Pull-down (NRST, BOOT0) | 0805 SMD |
| R1 | 1 | **220 Ω** | ±1% Current Limiting Resistor (LED) | 0805 SMD |
| **Capacitors** | | | | |
| C7, C8 | 2 | **10 µF** | Ceramic Capacitor (LDO Input/Output) | 0805 SMD |
| C1 | 1 | **1 µF** | Ceramic Capacitor (VDDA Filtering) | 0805 SMD |
| C3, C4, C5, C6, C9, C10 | 6 | **100 nF** | Ceramic Capacitor (Decoupling / Debouncing) | 0805 SMD |
| C2 | 1 | **10 nF** | Ceramic Capacitor (VDDA High-Freq Filter) | 0805 SMD |
| C11, C12 | 2 | **27 pF** | Ceramic Capacitor (8MHz Load) | 0805 SMD |
| C13, C14 | 2 | **18 pF** | Ceramic Capacitor (32kHz Load) | 0805 SMD |
