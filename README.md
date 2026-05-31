# Buck Converter Design and Simulation

## Overview
This project presents the design and simulation of a DC-DC Buck Converter operating in Continuous Conduction Mode (CCM). The converter steps down an input voltage ranging from 12 V to 15 V and provides a regulated output voltage of 8 V with a load power of 1.5 W.

## Objective
To design and analyze a Buck Converter operating in CCM that:
- Accepts an input voltage of 12–15 V
- Produces a regulated output voltage of 8 V
- Delivers an output power of 1.5 W
- Maintains stable operation with minimal voltage and current ripples

## Working Principle
A Buck Converter is a step-down DC-DC converter that uses:
- A switching device (MOSFET/Transistor)
- A freewheeling diode
- An inductor
- A capacitor

The inductor stores energy when the switch is ON and releases it when the switch is OFF. The capacitor filters the output voltage, reducing ripple and ensuring a stable DC output.

### Modes of Operation

#### Mode 1: Switch ON, Diode OFF
- The switch conducts current.
- The inductor stores energy in its magnetic field.
- The capacitor charges and supplies the load.

#### Mode 2: Switch OFF, Diode ON
- The switch blocks current.
- The inductor releases stored energy.
- The diode provides a path for current flow.
- The capacitor helps maintain a steady output voltage.

## Design Specifications

| Parameter | Value |
|------------|--------|
| Input Voltage (Vin) | 12 V |
| Output Voltage (Vo) | 8 V |
| Output Power (Po) | 1.5 W |
| Switching Frequency (f) | 10 kHz |
| Voltage Ripple | 1% |

## Design Calculations

### Duty Cycle
\[
D = \frac{V_o}{V_{in}} = \frac{8}{12} = 0.66
\]

### Load Resistance
\[
R = \frac{V_o^2}{P_o}
\]

\[
R = \frac{8^2}{1.5} = 42.66 \Omega
\]

Selected Resistance:
**43 Ω**

### Inductor Design

Calculated Inductance:

\[
L_{cal} = 0.711 \, mH
\]

Designed Inductance:

\[
L_{design} = 7.11 \, mH
\]

### Capacitor Design

Calculated Capacitance:

\[
C_{cal} = 0.058 \, mF
\]

Designed Capacitance:

\[
C_{design} = 0.58 \, mF
\]

## Simulation
The designed Buck Converter was simulated to verify:
- Output voltage regulation
- Continuous Conduction Mode operation
- Ripple reduction
- Stable performance under load conditions

## Applications
- Solar charging systems
- Mobile and laptop chargers
- Power banks
- Switch Mode Power Supplies (SMPS)
- Point-of-load converters in computers
- Adaptive control systems
- Audio power amplifiers

## Results
The designed Buck Converter successfully operates in Continuous Conduction Mode (CCM), converting an input voltage range of 12–15 V into a regulated 8 V output. The converter delivers 1.5 W of power while maintaining stable operation with reduced voltage and current ripples, making it suitable for low-power DC applications.

## Tools Used
- MATLAB/Simulink (if used)
- LTspice / Proteus / Multisim (if used)
- Hardware Components for prototype implementation

## Author
**Atchaya V**  
B.Tech Electrical and Electronics Engineering  
Amrita Vishwa Vidyapeetham
