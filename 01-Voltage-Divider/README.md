# ⚡ Voltage Divider — First PSpice Project

This is the first practical project of the **EEE Circuit Simulation Journey**.

The goal is to understand a simple voltage-divider circuit by following the complete engineering workflow:

**Understand → Calculate → Draw → Simulate → Verify**

---

## 🎯 Learning Objectives

By completing this project, we will learn how to:

- Understand a basic resistor circuit
- Apply Ohm's Law
- Calculate circuit current
- Calculate output voltage
- Calculate resistor power
- Draw a schematic in OrCAD X
- Run a PSpice simulation
- Measure simulation results
- Compare theoretical and simulated values

---

## 🔌 Circuit

The circuit consists of:

- One DC voltage source
- Two resistors
- Ground
- One output node

```text
              R1
      +10 V ─/\/\/───●───/\/\/─┐
                     │    R2    │
                     │          │
                   Vout         │
                     │          │
                     └──────────┘
                                GND
````

---

## 📐 Given Values

| Component           | Value |
| ------------------- | ----: |
| Voltage Source (Vs) |  10 V |
| R1                  |  1 kΩ |
| R2                  |  2 kΩ |

---

## 🧮 Theoretical Calculation

For a voltage-divider circuit:

$$
V_{out}=V_s\frac{R_2}{R_1+R_2}
$$

Substituting the given values:

$$
V_{out}=10\times\frac{2kΩ}{1kΩ+2kΩ}
$$

$$
V_{out}=6.67V
$$

Therefore, the theoretical output voltage is approximately:

**Vout ≈ 6.67 V**

---

## ⚡ Circuit Current

The total resistance is:

$$
R_{total}=R_1+R_2
$$

$$
R_{total}=1kΩ+2kΩ=3kΩ
$$

Using Ohm's Law:

$$
I=\frac{V_s}{R_{total}}
$$

$$
I=\frac{10V}{3kΩ}
$$

$$
I\approx3.33mA
$$

---

## 🔥 Power Calculation

For a resistor:

$$
P=I^2R
$$

We will calculate the power dissipated by both R1 and R2 and later verify the values using simulation.

---

# 💻 PSpice Simulation

The same circuit will now be recreated in **OrCAD X / PSpice**.

### Workflow

```text
Place Components
      ↓
Connect Wires
      ↓
Set Component Values
      ↓
Add Ground
      ↓
Create Simulation Profile
      ↓
Run PSpice
      ↓
Measure Vout
      ↓
Compare With Theory
```

---

## 📊 Expected Result

Before running the simulation, predict the result:

**Expected Vout ≈ 6.67 V**

After simulation, record the actual PSpice result here:

| Parameter | Theoretical | PSpice | Difference |
| --------- | ----------: | -----: | ---------: |
| Vout      |      6.67 V |      — |          — |
| Current   |     3.33 mA |      — |          — |
| P(R1)     |           — |      — |          — |
| P(R2)     |           — |      — |          — |

---

## 🔍 Verification

The purpose of simulation is not to replace mathematical analysis.

We first calculate the circuit manually and then use PSpice to verify our result.

### Engineering Workflow

**Manual Calculation**

↓

**PSpice Simulation**

↓

**Result Comparison**

↓

**Error Investigation**

---

## 🧪 Challenge

Change the resistor values and calculate the new output voltage before running PSpice.

### Challenge A

```text
Vs = 12 V
R1 = 2 kΩ
R2 = 4 kΩ
```

Find:

* Total current
* Vout
* Power of R1
* Power of R2

### Challenge B

```text
Vs = 5 V
R1 = 1 kΩ
R2 = 4.7 kΩ
```

Find:

* Total current
* Vout
* Power of R1
* Power of R2

**Do the calculations yourself before using PSpice.**

---

## 📁 Project Files

The project will eventually contain:

```text
01-Voltage-Divider/
│
├── README.md
├── schematic/
├── simulation/
├── results/
└── calculations/
```

Screenshots, PSpice project files, and simulation results will be added as the project progresses.

---

## 🧠 What We Learned

After completing the simulation, document:

* What was easy?
* What was difficult?
* Did the simulation match the calculation?
* If there was a difference, why?
* What did we learn about PSpice?

---

## 🚀 Next

After completing the voltage-divider project, the next project will introduce a slightly more complex circuit and continue the same workflow:

**Calculate → Draw → Simulate → Verify**

```

