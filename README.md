# STM32F103C8T6 Custom Development Board

A custom 4-layer printed circuit board (PCB) designed to house the STM32F103C8T6 ARM Cortex-M3 microcontroller. This project demonstrates the complete hardware development lifecycle, from modular schematic capture to high-density layout routing and manufacturing file generation.

Designed entirely in **Altium Designer**.

## Hardware Architecture & Specifications

### Microcontroller & Clocking
*   **MCU:** STMicroelectronics STM32F103C8T6 (ARM Cortex-M3 @ 72 MHz)
*   **High-Speed External (HSE):** 8MHz Crystal Oscillator matched with 27pF load capacitors for accurate main system clocking.
*   **Low-Speed External (LSE):** 32.768kHz Crystal matched with 18pF load capacitors for Real-Time Clock (RTC) functionality.

### Power Architecture & Filtering
*   **Input & Interface:** USB Type-C connector configured with dual 5.1kΩ CC-pin pull-down resistors for proper 5V power negotiation from modern hosts.
*   **Regulation:** AMS1117-3.3V Low Dropout (LDO) regulator stepping down the 5V USB input to a stable 3.3V power rail, stabilized with 10µF input and output ceramic capacitors.
*   **Decoupling Network:** Comprehensive localized filtering utilizing a centralized bank of bypass capacitors (10µF bulk alongside multiple 100nF high-frequency caps) to ensure clean power delivery.
*   **Analog Isolation:** Dedicated VDDA filtering utilizing 1µF and 10nF capacitors for precise analog-to-digital conversions.

### Protection & Control
*   **Transient Protection:** Dedicated ESD Protection IC placed directly on the USB data lines (DP/DN) to shield the MCU from electrostatic discharge events.
*   **Hardware Debouncing:** NRST (Reset) and BOOT0 push-buttons feature dedicated RC networks (10kΩ pull-up/pull-down resistors and 100nF capacitors) for clean, debounced signal transitions.

### Connectivity
*   **Programming:** Dedicated 4-pin ST-Link header (SWDIO, SWCLK, GND, +3V3) for serial wire debugging.
*   **Communication:** Dedicated 4-pin UART header for serial communication.
*   **I/O Breakout:** Comprehensive GPIO access via standardized 10-pin and 4-pin headers.

### PCB Stackup & Signal Integrity
The board utilizes a standard **4-layer stackup** to optimize signal integrity, impedance matching, and thermal dissipation:
*   **Layer 1 (Top):** High-speed signal routing and SMD components.
*   **Layer 2 (Internal 1):** Solid Ground (GND) plane for short return paths and EMI reduction.
*   **Layer 3 (Internal 2):** Dedicated Power (PWR) plane.
*   **Layer 4 (Bottom):** Low-speed signals and routing channels.

## 3D Visuals of The Board

<img width="700" height="581" alt="Screenshot 2026-08-28 154627" src="https://github.com/user-attachments/assets/06f51a54-b662-4a87-979c-155baff18248" /> <br><br>
<img width="584" height="660" alt="Screenshot 2026-08-28 154612" src="https://github.com/user-attachments/assets/9414a768-a623-458d-b048-68f49f6ee7b1" />


## Repository Contents
*   **`/Gerber_Files`**: Contains the complete manufacturing package (`.zip`) including copper layers, masks, silkscreens, board outline, and 4:4 precision NC Drill files ready for fabrication.
*   **`/Schematics`**: High-resolution PDF of the modular circuit design.
*   **`BOM.md`**: Complete Bill of Materials detailing component selection and footprint data.

---
*Designed by Amaar Ayman*
