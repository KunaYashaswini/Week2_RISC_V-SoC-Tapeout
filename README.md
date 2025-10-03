# Week2_RISC_V-SoC-Tapeout
# Fundamentals of SoC Design — VSDBabySoC Journey
## Problem Statement

VSDBabySoC is an open-source SoC based on the RVMYTH RISC-V core.
It integrates a PLL for stable clock generation and a 10-bit DAC for analog output, enabling interfacing with devices like TVs and mobiles.
Built on Sky130 technology, it serves as an educational platform for SoC and digital-analog interfacing.

### 1. What is an SoC?
A System on Chip (SoC) combines CPU, memory, I/O, GPU/DSP, power control, and special features on one chip.
#### Why Important?
Smaller, faster, and energy-efficient.
Lower cost and higher reliability.
#### Where Used?
Smartphones, tablets, wearables, IoT devices, cars, TVs.
#### Challenges
Complex design, heat issues, and less flexibility after fabrication.

### 2. Types of SoCs

#### Microcontroller-based: 
Low power, simple control (IoT, appliances).

#### Microprocessor-based: 
Runs OS, multitasking (phones, tablets).

#### Application-Specific: 
Optimized for special tasks (AI, graphics, networking).

### 3. VSDBabySoC

A compact SoC to test CPU, PLL, and DAC together.

#### Components

#### RVMYTH CPU:
Processes data.

#### PLL:
Generates stable clock.

#### DAC:
Converts digital data to analog output.

#### Flow
1.PLL locks clock.
2.CPU updates register r17.
3.DAC converts values → analog output (OUT file).

### 4. Phase-Locked Loop (PLL)
Phase Detector → Loop Filter → VCO with feedback.
Keeps clock stable and synchronized.
Needed to handle jitter, delay, and frequency errors in off-chip clocks.
![My Screenshot](ChatGPT%20Image%20Oct%203%2C%202025%2C%2009_58_43%20PM.png)
### 5. Digital-to-Analog Converter (DAC)
Converts binary values to analog signals.
Types: Weighted Resistor, R-2R Ladder.
In BabySoC: 10-bit DAC produces audio/video signals from CPU data.

### Conclusion
VSDBabySoC demonstrates how a small SoC with CPU + PLL + DAC can generate real-world analog outputs.
It’s a hands-on learning platform for SoC fundamentals, RISC-V, and Sky130 open-source design.
