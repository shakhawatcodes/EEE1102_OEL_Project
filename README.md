# EEE1102 OEL Project

## Verification of Thevenin's Theorem, Maximum Power Transfer Theorem & Superposition Theorem

**Course:** EEE1102
**Project Type:** Operational Engineering Laboratory (OEL)
**Student No.:** 00725205131037
**Student:** Shakhawat Hossain
**Institution:** AUST
---

## 📌 Project Overview

This project presents the design, simulation, analysis, and verification of a unique DC resistive circuit containing **30–35 standard-value resistors and two independent voltage sources**.

The circuit is analyzed to determine its **Thevenin Equivalent Circuit** with respect to a selected pair of terminals. The Thevenin resistance is determined using **three different methods**, and the results are compared for verification.

The project also investigates the behavior of a variable load resistance connected across the selected terminals and verifies:

* **Thevenin's Theorem**
* **Maximum Power Transfer Theorem**
* **Superposition Theorem**

The complete simulation data, circuit files, graphs, and supporting files are included in this repository.

---

## 🎯 Objectives

The major objectives of this project are:

1. To design a unique DC circuit containing **30–35 resistors** and **two voltage sources**.
2. To select and denote two terminals for Thevenin equivalent analysis.
3. To determine the **Thevenin voltage \(V_{th}\)** across the selected terminals.
4. To determine the **Thevenin resistance \(R_{th}\)** using three different methods.
5. To construct the corresponding Thevenin equivalent circuit.
6. To connect a variable load resistance \(R_L\) across the original circuit and Thevenin equivalent circuit.
7. To obtain:

   * \(V_L\) vs. \(R_L\)
   * \(I_L\) vs. \(R_L\)
   * \(P_L\) vs. \(R_L\)
8. To verify **Thevenin's Theorem**.
9. To verify the **Maximum Power Transfer Theorem**.
10. To verify **Superposition Theorem** for both voltage and current across a selected resistor.
11. To compare simulation results with theoretical calculations.
12. To document all relevant measurements, graphs, circuit designs, and calculations.

---

# ⚡ Circuit Design

The main circuit consists of:

* **30–35 standard/medium-value resistors**
* **2 independent DC voltage sources**
* Selected output terminals for Thevenin analysis
* A variable load resistance \(R_L\)

The voltage sources are selected within the recommended range of approximately **25–30 V**, while the resistor values are chosen from practical standard values.

### Circuit Requirements

| Parameter            | Requirement            |
| -------------------- | ---------------------- |
| Number of resistors  | 30–35                  |
| Voltage sources      | 2                      |
| Resistor type        | Standard/medium value  |
| Voltage source range | Approximately 25–30 V  |
| Load                 | Variable \(R_L\)       |
| Analysis terminals   | Two selected terminals |
| Simulation           | DC circuit analysis    |

---

# 🔬 Thevenin's Theorem

For the selected pair of terminals, the original network is replaced by an equivalent circuit consisting of:

* Thevenin voltage \(V_{th}\)
* Thevenin resistance \(R_{th}\)
* Variable load resistance \(R_L\)

The load voltage and current are determined from both the **original circuit** and the **Thevenin equivalent circuit** and compared for verification.

### Thevenin Equivalent

$$
V_L = V_{th}\frac{R_L}{R_{th}+R_L}
$$

$$
I_L = \frac{V_{th}}{R_{th}+R_L}
$$

$$
P_L = V_L I_L
$$

---

# 🧮 Determination of Thevenin Resistance

The project determines \(R_{th}\) using **three independent methods**.

### Method 1 — Equivalent Resistance Method

The network is simplified using series and parallel resistor combinations to obtain the equivalent resistance seen from the selected terminals.

### Method 2 — Source Deactivation Method

The independent voltage sources are deactivated by replacing ideal voltage sources with short circuits.

The resistance seen from the selected terminals is then calculated:

$$
R_{th}=R_{eq}
$$

### Method 3 — Open-Circuit Voltage / Short-Circuit Current Method

The Thevenin resistance is determined using:

$$
R_{th}=\frac{V_{OC}}{I_{SC}}
$$

where:

* \(V_{OC}\) = open-circuit voltage
* \(I_{SC}\) = short-circuit current

The three calculated values are compared with the simulation result.

---

# 📊 Variable Load Analysis

A variable load resistance \(R_L\) is connected across the selected terminals.

The load resistance is varied over an appropriate range and step size.

For every value of \(R_L\), the following parameters are measured:

* Load voltage \(V_L\)
* Load current \(I_L\)
* Load power \(P_L\)

The same measurements are obtained for both:

1. Original circuit
2. Thevenin equivalent circuit

---

# 📈 Graphical Analysis

The following graphs are generated from the simulation measurements:

### 1. Load Voltage vs. Load Resistance

$$
V_L \text{ vs. } R_L
$$

### 2. Load Current vs. Load Resistance

$$
I_L \text{ vs. } R_L
$$

### 3. Load Power vs. Load Resistance

$$
P_L \text{ vs. } R_L
$$

The graphs for the original circuit and Thevenin equivalent circuit are compared to verify that both circuits produce equivalent terminal behavior.

---

# ⚙️ Maximum Power Transfer Theorem

The Maximum Power Transfer Theorem states that maximum power is delivered to the load when:

$$
R_L=R_{th}
$$

At this condition:

$$
P_{max}=\frac{V_{th}^{2}}{4R_{th}}
$$

The \(P_L\) vs. \(R_L\) graph is used to identify the load resistance corresponding to maximum power.

The experimentally/simulation-obtained value is compared with the theoretical condition:

$$
R_L \approx R_{th}
$$

---

# 🔄 Superposition Theorem

Since the circuit contains **two independent voltage sources**, the Superposition Theorem is verified.

The response of the circuit is analyzed under three conditions:

### Case 1 — Both Sources Active

Both voltage sources are active and the required voltage/current is measured.

### Case 2 — Source 1 Active

The second independent voltage source is deactivated by replacing it with a short circuit.

The required voltage/current is measured.

### Case 3 — Source 2 Active

The first independent voltage source is deactivated by replacing it with a short circuit.

The required voltage/current is measured.

The individual contributions are then added algebraically:

$$
V = V_1+V_2
$$

$$
I = I_1+I_2
$$

The result is compared with the response obtained when both sources are active.

---

# 📋 Measurements

The project contains measurement data for the following parameters:

| Analysis               | Parameters                         |
| ---------------------- | ---------------------------------- |
| Original Circuit       | \(V_L, I_L, P_L\)                  |
| Thevenin Circuit       | \(V_L, I_L, P_L\)                  |
| Thevenin Analysis      | \(V_{OC}, I_{SC}, V_{th}, R_{th}\) |
| Maximum Power Transfer | \(R_L, P_{max}\)                   |
| Superposition          | Voltage and current contributions  |
| Load Analysis          | Multiple \(R_L\) values            |

Detailed measurement tables and calculations are included in the final report.

---

# 📁 Repository Contents

The repository contains the simulation and supporting files generated during the project.

```text
EEE1102_OEL_Project/
│
├── OELSim1102_00725205131037_a.asc
├── OELSim1102_00725205131037_b.asc
├── OELSim1102_00725205131037_c.asc
├── OELSim1102_00725205131037_d.asc
├── OELSim1102_00725205131037_e.asc
├── OELSim1102_00725205131037_f.asc
├── OELSim1102_00725205131037_g.asc
├── OELSim1102_00725205131037_h.asc
├── OELSim1102_00725205131037_i.asc
│
├── *.log
├── *.raw
├── *.plt
├── *.net
│
└── README.md
```

### File Types

| Extension | Purpose                           |
| --------- | --------------------------------- |
| `.asc`    | Circuit schematic/simulation file |
| `.raw`    | Simulation raw data               |
| `.log`    | Simulation output/log information |
| `.plt`    | Plot configuration/data           |
| `.net`    | Netlist                           |
| `.md`     | Project documentation             |

---

# 🖥️ Simulation Software

The circuit simulations and analysis files are prepared using **LTspice**.

The `.asc` files can be opened and simulated using LTspice.

---



# ✅ Verification Summary

The project verifies the following fundamental circuit theorems:

| Theorem                | Verification                               |
| ---------------------- | ------------------------------------------ |
| Thevenin's Theorem     | Original and equivalent circuits compared  |
| Thevenin Resistance    | Determined using 3 methods                 |
| Maximum Power Transfer | \(P_L\) vs. \(R_L\) analysis               |
| Superposition Theorem  | Voltage and current contributions compared |

---

# 👨‍🎓 Student Information

**Student Name:** Shakhawat Hossain


**Student ID:** 00725205131037


**Course:** EEE1102

**Project:** Open Ended Laboratory (OEL)


**Institution:**  Ahsanullah University Of Science and Technology
---

## 📌 Note

This repository is intended to document the circuit simulation files, measurement data, analysis, and supporting materials for the EEE1102 OEL project.

The circuit is designed specifically for this project and the simulation files are provided for documentation and verification purposes.

