# 🔁 3-Stage Ring Oscillator – Schematic and Layout using Electric VLSI

This repository contains the **schematic and layout design** of a **3-stage ring oscillator** built using the free and open-source **Electric VLSI Design System**.

---

## 📌 What is a 3-Stage Ring Oscillator?

A 3-stage ring oscillator is a digital circuit formed by connecting an odd number of inverters in a loop. It generates a periodic oscillating signal without any external clock input.

---

## ✨ Features

- ✅ Designed using **Electric VLSI (Free and Open Source Tool)**
- ✅ Includes both **schematic** and **layout**
- ✅ Built using **CMOS inverter stages**
- ✅ Easy to simulate and expand further (e.g., into timing analysis, layout vs. schematic checks)
- ✅ DRC/LVS/ERC passed successfully. 
- ✅ 180nm Technology Node used.

---

## 🧠 Project Structure

```plaintext
📁 3-Stage-Ring-Oscillator-ElectricVLSI
├── ring_osc.sch        # Schematic file
├── ring_osc.lay        # Layout file
└── README.md           # Project documentation
```
## 🛠️ Design Workflow in Electric VLSI
### 1. 🧩 Schematic Design
- Open Electric VLSI
- Create a new cell and choose schematic view
- Use three CMOS inverters (each made with pMOS + nMOS)
- Connect the inverters in series
- Feed the output of the third inverter back to the input of the first
- Add power rails: vdd and gnd
- Validate connections using built-in Electric checks

### 2. 🧱 Layout Design
- Create another new cell and choose layout view
- Design each inverter with:
- pMOS on top (in p-well)
- nMOS on bottom (in n-well)

#### Use:

- Diffusion, Polysilicon, Metal1
- Contacts to interconnect layers
- Replicate the inverter layout 3 times
- Connect them in a feedback loop
- Place vdd and gnd metal rails
- Ensure clean layout and connectivity

## 🔄 How It Works
The oscillator works due to the odd number of inverting stages creating instability that leads to periodic toggling.

The delay of each inverter contributes to the oscillation frequency.

Frequency formula (ideal):

f = 1/(2*N*tp)
​
where:

N = number of inverter stages (3 here)

t_p = propagation delay of a single inverter

## 📌 Requirements
- Electric VLSI Tool (https://staticfreesoft.com/productsFree.html)
- Java Runtime Environment (for Electric VLSI)

## 🚀 Future Scope
- ✅ Add SPICE netlist export and simulate using Ngspice or LTspice
- ✅ Expand to 5-stage or 7-stage oscillator
- ✅ Measure power and delay characteristics

If any query, don't hasistate to connect with me on:

- Gmail: dattpanchal2904@gmail.com
- GitHUb: https://github.com/DuttPanchal04
- LinkedIn: https://www.linkedin.com/in/dattpanchal04/

Thank you!