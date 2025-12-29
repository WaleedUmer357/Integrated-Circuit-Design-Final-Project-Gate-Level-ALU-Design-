# Integrated-Circuit-Design-Final-Project-Gate-Level-ALU-Design-
I designed an industrial grade vlsi design of an ALU.
# 4-bit Arithmetic Logic Unit (ALU) - VLSI Design Project

 📋 Project Overview
This project involves the design and implementation of a 4-bit Arithmetic Logic Unit (ALU) as part of the Integrated Circuit Design program at Griffith University. The ALU supports eight operations including addition, subtraction, logical shifts, negation, absolute value, multiplication, and minimum selection. The design focuses on optimizing delay, area, and power consumption using the Electric VLSI Design System.



 🛠️ Features
- 8 Operations Supported:
  1. Addition (A + B)
  2. Subtraction (A – B)
  3. Left shift B
  4. Negative A (two’s complement)
  5. Negative B (two’s complement)
  6. Absolute (|A – B|)
  7. Multiplication (A × B) – 8-bit output
  8. Minimum selector (Min(A, B))

- Inputs:
  - 4-bit A (A0–A3)
  - 4-bit B (B0–B3)
  - 3-bit selector (S2, S1, S0)

- Outputs:
  - 4-bit R (R0–R3) for most operations
  - 8-bit R (R0–R7) for multiplication
  - Carry (cout) and Overflow (V) flags for arithmetic operations



 🔧 Design Highlights
# 1. Transistor Sizing
- pMOS width = 2 × nMOS width to balance mobility and switching thresholds.
- Minimum transistor length = 2λ (MOSIS CMOS technology).

# 2. Gate-Level Optimizations
- Used NAND gates instead of AND/OR gates for lower logical effort and reduced area.
- Designed custom XOR gates and full adders for improved speed and power efficiency.

# 3. Layout Strategies
- Inputs and outputs placed on opposite sides to reduce wire length and crosstalk.
- Wire shielding and increased spacing to minimize interference.
- Used π-model for long wires to reduce RC delay.

# 4. Power Optimization
- Dynamic power reduction through:
  - Smaller pin sizes (lower capacitance).
  - Shorter wires and efficient multiplexer design.
  - Organized power (VDD) and ground (GND) distribution using Metal 3.



 📁 Project Structure
```
📦 ALU-Design-Project
├── 📄 README.md
├── 📂 schematics/          # Electric schematic files (.sch)
├── 📂 layouts/             # Electric layout files (.lay)
├── 📂 simulations/         # Simulation waveforms and testbenches
├── 📂 stimuli/             # Input stimuli files for verification
├── 📂 docs/                # Project report and references
└── 📂 appendix/            # Additional gates and block designs




 ⚙️ Simulation & Verification
- Tools Used: Electric VLSI Design System
- Checks Performed:
  - Design Rule Check (DRC)
  - Electrical Rule Check (ERC)
  - Netlist Connectivity Check (NCC)
- Simulation Results:
  - All blocks verified with delay < 2 ns.
  - Final ALU delay ≈ 1.5 ns.



 📊 Performance Metrics
- Delay: < 2 ns per block
- Area: Optimized through gate reuse and compact layout
- Power: Reduced via pin sizing, wire optimization, and efficient multiplexing



 🚧 Known Issues & Future Work
- Multiplier currently not fully functional in final integration (pin connection issue).
- Further optimization possible in wire routing to reduce delay.
- Plan to implement Booth’s algorithm for multiplier enhancement.



 📚 References
1. Weste, N.H.E. & Harris, D.M. – Integrated Circuit Design
2. Stan, M.R. – Optimal Voltages and Sizing for Low Power
3. Singh et al. – Optimum Transistor Sizing Using Logical Effort Theory
4. Raj & Syamala – Transistor Level Implementation of Digital Reversible Circuits



 👤 Author
Waleed Umer  
Griffith University  


