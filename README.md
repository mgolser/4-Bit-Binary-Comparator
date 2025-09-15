# 4-bit Comparator with 7-Segment Display

## Overview
This circuit implements a **4-bit magnitude comparator** using basic logic gates in Wokwi.  
Two 4-bit values (A and B) are entered via the DIP switch. The logic compares whether **A > B** and outputs the result to a 7-segment display.

## Inputs
- **A_3…A_0** → 4-bit number **A** (`A_3 = MSB`, `A_0 = LSB`)  
  - Switch 1 → `A_3` (MSB)  
  - Switch 2 → `A_2`  
  - Switch 3 → `A_1`  
  - Switch 4 → `A_0` (LSB)  

- **B_3…B_0** → 4-bit number **B** (`B_3 = MSB`, `B_0 = LSB`)  
  - Switch 5 → `B_3` (MSB)  
  - Switch 6 → `B_2`  
  - Switch 7 → `B_1`  
  - Switch 8 → `B_0` (LSB)  

## Outputs
- The comparator result is routed through `SEG_*` pins to the 7-segment display.  
- The display shows:  
  - **“1”** → if A > B  
  - **“0”** → otherwise (A ≤ B)  

## How to Use
Flip the DIP switches to set binary values for A and B.  

- Left group Switches (1–4) → Inputs `A_3–A_0` for **A**  
- Right group Switches (5–8) → Inputs `B_3–B_0` for **B**  

The comparator logic evaluates A and B in real time, and the 7-segment display immediately shows the result of the comparison.
