# EEE1102 OEL Project

## Verification of Thevenin's Theorem, Maximum Power Transfer Theorem & Superposition Theorem

**Course:** EEE1102
**Project Type:** Open Ended Lab (OEL)
**Student No.:** 00725205131037
**Student:**  Mohammad Shakhawat Hossain
**Institution:** Ahsanullah University of Science and Technology

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

The Thevenin re
