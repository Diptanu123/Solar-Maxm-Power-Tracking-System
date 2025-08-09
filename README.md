# ☀️ Solar Maximum Power Tracking System

## 📌 Overview
The **Solar Maximum Power Tracking System** is designed to ensure that a solar panel is always aligned with the sun’s position, maximizing energy generation throughout the day.  
Using **Arduino Uno**, **LDR sensors**, and a **servo motor**, the system detects the sun’s position and adjusts the panel’s orientation accordingly.

---

## ✨ Key Features
- Tracks sun’s position automatically in real time.
- Maximizes solar panel output by optimal alignment.
- Uses **Light Dependent Resistors (LDRs)** for light intensity sensing.
- Low-cost and energy-efficient design.
- Scalable for larger solar farms or personal solar setups.

---

## 🛠 Components Used
| Component              | Quantity | Description |
|------------------------|----------|-------------|
| Arduino Uno            | 1        | Microcontroller board |
| Servo Motor            | 1        | Rotates the solar panel |
| Solar Panel            | 1        | Generates electricity |
| LDR (Light Sensor)     | 2        | Detects sunlight intensity |
| Resistors (10kΩ)       | 2        | Acts as pull-down resistors |
| Cardboard / Base Frame | 1        | Panel mounting structure |
| Jumper Wires           | As needed | Connections |
| Glue Gun               | 1        | Assembly fixing |

---

## ⚙️ How It Works
1. **Light Detection:**  
   Two LDRs are placed on opposite sides of the solar panel to measure light intensity.
   
2. **Signal Processing:**  
   Arduino reads LDR values via analog pins **A0** and **A1**.

3. **Position Adjustment:**  
   - If light intensity is higher on the east LDR → Servo rotates panel east.  
   - If light intensity is higher on the west LDR → Servo rotates panel west.  
   - If both LDRs detect low light → Panel resets towards east (sunrise position).

4. **Servo Motor Control:**  
   The servo motor adjusts its position according to the calculated light intensity difference (`error = east - west`).

---

## 🔍 Applications
- Solar farms for large-scale renewable energy.
- Home solar power systems.
- Solar-powered street lights.
- Remote area solar power installations.

---

## 🚀 Future Improvements
- Use **high-torque servo motors** for larger panels.
- Replace cardboard with **aluminum or steel** for durability.
- Add **dual-axis tracking** for seasonal tilt adjustments.
- Integrate with **IoT for remote monitoring**.

---

## 🖥 Circuit Diagram
*(Insert your circuit schematic image here)*

**Connections:**
- LDR1 → Analog Pin A0  
- LDR2 → Analog Pin A1  
- Servo Motor → Pin 9  
- Power → 5V (from Arduino)  
- Resistors (10kΩ) → Pull-down configuration  

---
