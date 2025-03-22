# Digital Railway Timer

## Project Overview
The Digital Railway Timer is a logic gate-based digital clock designed to display time in a 24-hour format (00:00 to 23:59) accurately tracks hours and minutes. The project prioritizes simplicity, efficiency, and low power consumption in its logic circuitry.

## Features
- Displays time in a **24-hour format** (00:00 - 23:59)
- Uses **logic gates and BCD counters** for accurate time tracking
- Handles transitions between **AM and PM seamlessly**
- Optimized for **low power consumption and efficient logic design**
- Uses **7-segment displays** for clear visibility

## Components Required
- **IC 555 Timer** (1x) – Clock signal generator
- **CD4518 Dual Up Counter** (2x) – BCD counters for minute and hour calculations
- **74LS47 (7-Segment Display Driver)** (4x) – Driving 7-segment displays
- **7-Segment Display** (4x) – Displaying hours and minutes
- **Basic Logic Gates** – Used for logic control
- **Breadboard & Wires** – Circuit assembly

## Implementation Details
### Minute Calculation
- A **555 timer** generates a clock pulse fed to the **CD4518 BCD counter**.
- The BCD counter tracks minute units and resets after reaching **59**.
- A **BCD to 7-segment decoder (CD7447)** converts the output for display.

### Hour Calculation
- Another **CD4518 BCD counter** tracks hour values, resetting after **23:59**.
- Logical conditions ensure **accurate AM/PM transitions**.
- The output is decoded using **CD7447**, driving the **7-segment display**.

## Circuit & HDL Implementation
- The circuit consists of **BCD counters, logic gates, and display drivers**.
- The Verilog **HDL code** provides a structured approach for digital design.

## Expected Output
- **Accurate time display** on **four 7-segment displays**.
- Seamless transition between **23:59 to 00:00** and between **AM and PM**.
- Efficient, **logic-based timekeeping** without the need for microcontrollers.

## Conclusion
This Digital Railway Timer provides a reliable **hardware-based solution** for accurate timekeeping in railway systems. By utilizing **logic gates and BCD counters**, it ensures efficiency, simplicity, and **low power consumption**, making it a practical and robust digital clock solution.


