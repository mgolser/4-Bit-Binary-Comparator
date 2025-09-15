# 4-bit Comparator with 7-Segment Display

## Overview
This circuit implements a **4-bit magnitude comparator** using basic logic gates in Wokwi.  
Two 4-bit values (A and B) are entered via the DIP switch (`sw1`). The logic compares whether **A > B** and outputs the result to a 7-segment display.

### Inputs
- `ttin:IN0…IN3` → 4-bit number **A** (`IN0 = MSB`, `IN3 = LSB`)  
- `ttin:IN4…IN7` → 4-bit number **B** (`IN4 = MSB`, `IN7 = LSB`)  

### Outputs
- The comparator result is routed through `ttout:OUTx` pins to the 7-segment display.  
- The display shows:  
  - **“1”** → if A > B  
  - **“0”** → otherwise (A ≤ B)  

## How to Use
Flip the DIP switches (`sw1`) to set binary values for A and B.  

- Left group (`IN0–IN3`) sets **A**  
- Right group (`IN4–IN7`) sets **B**  

The comparator logic evaluates A and B in real time, and the 7-segment display immediately shows the result of the comparison.
