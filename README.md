

# 3T Multi-bit RRAM for In-Memory Computing

This repository contains simulation files and documentation for a project focused on **designing and characterizing 3-terminal multi-bit Resistive RAM (RRAM)** devices for **in-memory computing (IMC)** applications, implemented using Cadence tools.


## 📌 Key Features

- **3T RRAM Cell Design**: Enables single-cycle MAC operations unlike 2T RRAM which needs 3 cycles (initialize, compute, read).
- **Multi-bit Storage**: Stores 2 bits per cell using Intermediate Resistance States (IRS), enhancing density and analog computation accuracy.
- **Cadence Simulation**: Transient and DC simulations performed for:
  - I–V characterization
  - State-dependent resistance programming
  - 3×3 crossbar array performing vector-matrix multiplication (VMM)

## 🧪 Resistance State Levels

| State | Resistance (Ω) |
|-------|----------------|
| 1     | 250            |
| 2     | 500            |
| 3     | 1000           |
| 4     | 10000          |

Programming is governed by voltage thresholds with positive voltages increasing and negative voltages decreasing the resistance state.

## ⚙️ VMM Simulation Example

For a 3×3 MAC unit with input voltages \( V_i = 0.8V \), and resistances \( R_1 = 250 \Omega, R_2 = 500 \Omega, R_3 = 1000 \Omega \), the output current is:

\[
I = 0.2 \left( \frac{0.8}{250} + \frac{0.8}{500} + \frac{0.8}{1000} \right) = 1.12 \text{ mA}
\]

## 🔧 Tools Used

- **Cadence Virtuoso** for schematic and transient simulations
- **Verilog-A**  for custom memory device modeling

## 👨‍🔬 Contributors

- [Sushant Gudmewar](https://github.com/sushantgudmewar)
- Pavani Tirunagiri  
- [Raghavpravin K S](https://github.com/RaghavpravinKS)
*(Course Project under Prof. Sandip Lashkare - EE658: Memory Device Technologies and Applications, IIT Gandhinagar)*

## 📚 References

1. [IEEE Xplore Article on 3T RRAM](https://ieeexplore.ieee.org/document/9145738/)
2. [Overview on RRAM - Springer](https://link.springer.com/article/10.1186/s11671-020-03299-9)
3. [Forming-free Bipolar Switching - ScienceDirect](https://www.sciencedirect.com/science/article/abs/pii/S0022369722001172)

---

**Note**: This repository is academic in nature and intended for educational and research purposes.

