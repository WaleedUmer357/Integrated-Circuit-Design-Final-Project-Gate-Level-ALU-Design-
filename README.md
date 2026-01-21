<h3>🔬 VLSI & IC Design</h3>

- <b><a href="https://github.com/WaleedUmer357/Integrated-Circuit-Design-Final-Project-Gate-Level-ALU-Design-">4-bit Arithmetic Logic Unit (ALU) - VLSI Design Project</a></b>
  - Industrial-grade VLSI design of an ALU
  - <a href="https://github.com/WaleedUmer357/Integrated-Circuit-Design-Final-Project-Gate-Level-ALU-Design-/tree/main/ICD%20Design%20Project/ICD_Design_Project/jelib_project%20files">Design Files</a> | <a href="https://github.com/WaleedUmer357/Integrated-Circuit-Design-Final-Project-Gate-Level-ALU-Design-/tree/main/ICD%20Design%20Project/ICD_Design_Project/Result_images">Simulation Results</a> | <a href="https://github.com/WaleedUmer357/Integrated-Circuit-Design-Final-Project-Gate-Level-ALU-Design-/tree/main/ICD%20Design%20Project/ICD_Design_Project/Results">Layout</a>
  
  <details>
  <summary>📋 Click to view Project Details</summary>
  <br>
  
  <h4>Project Overview</h4>
  <p>This project involves the design and implementation of a 4-bit Arithmetic Logic Unit (ALU) as part of the Integrated Circuit Design program at Griffith University. The ALU supports eight operations including addition, subtraction, logical shifts, negation, absolute value, multiplication, and minimum selection. The design focuses on optimizing delay, area, and power consumption using the Electric VLSI Design System.</p>
  
  <h4>Features</h4>
  <p><b>8 Operations Supported:</b></p>
  <ol>
    <li>Addition (A + B)</li>
    <li>Subtraction (A – B)</li>
    <li>Left shift B</li>
    <li>Negative A (two's complement)</li>
    <li>Negative B (two's complement)</li>
    <li>Absolute (|A – B|)</li>
    <li>Multiplication (A × B) – 8-bit output</li>
    <li>Minimum selector (Min(A, B))</li>
  </ol>
  
  <p><b>Inputs:</b></p>
  <ul>
    <li>4-bit A (A0–A3)</li>
    <li>4-bit B (B0–B3)</li>
    <li>3-bit selector (S2, S1, S0)</li>
  </ul>
  
  <p><b>Outputs:</b></p>
  <ul>
    <li>4-bit R (R0–R3) for most operations</li>
    <li>8-bit R (R0–R7) for multiplication</li>
    <li>Carry (cout) and Overflow (V) flags for arithmetic operations</li>
  </ul>
  
  <h4>Design Highlights</h4>
  
  <p><b>Transistor Sizing</b></p>
  <ul>
    <li>pMOS width = 2 × nMOS width to balance mobility and switching thresholds</li>
    <li>Minimum transistor length = 2λ (MOSIS CMOS technology)</li>
  </ul>
  
  <p><b>Gate-Level Optimizations</b></p>
  <ul>
    <li>Used NAND gates instead of AND/OR gates for lower logical effort and reduced area</li>
    <li>Designed custom XOR gates and full adders for improved speed and power efficiency</li>
  </ul>
  
  <p><b>Layout Strategies</b></p>
  <ul>
    <li>Inputs and outputs placed on opposite sides to reduce wire length and crosstalk</li>
    <li>Wire shielding and increased spacing to minimize interference</li>
    <li>Used π-model for long wires to reduce RC delay</li>
  </ul>
  
  <p><b>Power Optimization</b></p>
  <ul>
    <li>Dynamic power reduction through:
      <ul>
        <li>Smaller pin sizes (lower capacitance)</li>
        <li>Shorter wires and efficient multiplexer design</li>
        <li>Organized power (VDD) and ground (GND) distribution using Metal 3</li>
      </ul>
    </li>
  </ul>
  
  <h4>Simulation & Verification</h4>
  <ul>
    <li><b>Tools Used:</b> Electric VLSI Design System</li>
    <li><b>Checks Performed:</b>
      <ul>
        <li>Design Rule Check (DRC)</li>
        <li>Electrical Rule Check (ERC)</li>
        <li>Netlist Connectivity Check (NCC)</li>
      </ul>
    </li>
    <li><b>Simulation Results:</b>
      <ul>
        <li>All blocks verified with delay &lt; 2 ns</li>
        <li>Final ALU delay ≈ 1.5 ns</li>
      </ul>
    </li>
  </ul>
  
  <h4>Performance Metrics</h4>
  <table>
    <tr>
      <td><b>Delay</b></td>
      <td>&lt; 2 ns per block</td>
    </tr>
    <tr>
      <td><b>Area</b></td>
      <td>Optimized through gate reuse and compact layout</td>
    </tr>
    <tr>
      <td><b>Power</b></td>
      <td>Reduced via pin sizing, wire optimization, and efficient multiplexing</td>
    </tr>
  </table>
  
  <h4>Design Images & Results</h4>
  
  <p><b>Schematic Design</b></p>
  <img src="Images/ALU Schematic.png" alt="ALU Schematic" width="700"/>
  
  <p><b>Layout Design</b></p>
  <img src="Images/ALU Layout.png" alt="ALU Layout" width="700"/>
  
  
  <p><b>Full Adder Design</b></p>
  <img src="Images/Full Adder Design.png" alt="Full Adder" width="500"/>
  
  <p><b>Multiplexer Design</b></p>
  <img src="Images/Multiplexer Design.png" alt="Multiplexer" width="500"/>
  
  <h4>Known Issues & Future Work</h4>
  <ul>
    <li>Multiplier currently  functional in final integration but can be better optimized(pin connection issue)</li>
    <li>Further optimization possible in wire routing to reduce delay</li>
    <li>Plan to implement Booth's algorithm for multiplier enhancement</li>
  </ul>
  
  <h4>References</h4>
  <ol>
    <li>Weste, N.H.E. & Harris, D.M. – Integrated Circuit Design</li>
    <li>Stan, M.R. – Optimal Voltages and Sizing for Low Power</li>
    <li>Singh et al. – Optimum Transistor Sizing Using Logical Effort Theory</li>
    <li>Raj & Syamala – Transistor Level Implementation of Digital Reversible Circuits</li>
  </ol>
  
  <p><b>Author:</b> Waleed Umer | Griffith University</p>
  
  </details>
