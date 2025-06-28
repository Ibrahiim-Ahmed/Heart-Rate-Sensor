## 💓 Heart Rate Monitor – Pure Digital Logic Implementation

This project demonstrates a **heart rate monitoring system** built **entirely using digital electronics components** such as logic gates, flip-flops, comparators, and 7-segment display ICs — with **no microcontroller, Arduino, Raspberry Pi, or programmable logic** involved. It showcases how fundamental principles of digital electronics can be applied to create a functional and educational biomedical device.

### 🧠 Project Overview

The Heart Rate Monitor works by detecting the user's heartbeat using a basic **infrared-based photoplethysmography (PPG) technique**. Blood flow changes in the fingertip cause variations in light absorption, which are captured as analog pulses. These pulses are processed through comparators and converted into clean digital signals.

Using only **digital logic ICs**, the system counts the number of heartbeats in a fixed time interval and then calculates the **beats per minute (BPM)**. The resulting BPM value is displayed using **7-segment displays** to give a real-time readout of the user’s heart rate.

---

## 🧩 Component List and Their Functions

| **Component**                                                   | **Purpose / Function**                                                                                                 |
| --------------------------------------------------------------- | ---------------------------------------------------------------------------------------------------------------------- |
| **IR LED + Photodiode/Phototransistor**                         | Forms the basic **PPG sensor** to detect heartbeat by sensing blood volume changes in the fingertip.                   |
| **LM358 / LM324 Comparator IC**                                 | Converts the **analog signal** from the PPG sensor into a clean **digital pulse** signal based on a voltage threshold. |
| **555 Timer (Monostable Mode)**                                 | Generates a **uniform pulse width** for each heartbeat detected, ensuring consistent pulse counting.                   |
| **D Flip-Flops (e.g., 74LS74)**                                 | Used to create **edge detectors**, **counters**, or **pulse synchronizers** to stabilize and process heartbeats.       |
| **Binary Counter ICs (e.g., 74LS90 / 74LS93)**                  | Counts the number of heartbeats in a predefined time window (e.g., over 6 or 10 seconds).                              |
| **AND, OR, NOT, XOR Gates (74LS Series)**                       | Implements **control logic** for counting, reset, gating, and display enable functions.                                |
| **BCD to 7-Segment Decoder (e.g., 74LS47 or CD4511)**           | Converts binary count values to **7-segment compatible signals** for readable display.                                 |
| **7-Segment Display**                                           | Displays the **BPM value** (or scaled count value) to the user. Usually 2 or 3 digits used.                            |
| **Multiplexers (e.g., 74LS157 or 74LS138)**                     | (Optional) Used for **digit selection** in case of a time-multiplexed multi-digit display.                             |
| **Clock Generator (Crystal Oscillator or 555 in Astable Mode)** | Provides the **reference timing clock** for counting the duration (e.g., 1Hz clock for 1s timing window).              |
| **Capacitors and Resistors**                                    | Used for **timing**, **filtering**, **biasing**, and **sensor conditioning** in analog sections.                       |
| **Push Button / Switch**                                        | For **manual reset** of the counter or to start/stop counting cycles.                                                  |

---

### ⏱️ How the Timing Works:

* Count the number of digital pulses (heartbeats) in a fixed time window (e.g., 10 seconds).
* Multiply the count by 6 to approximate BPM.
* Alternatively, adjust clock frequency and counters to scale the output automatically to BPM.

---


### 🔧 Key Features

* 📟 **Real-time Heart Rate Display** (in BPM) using 7-segment displays
* ⏱️ **Digital pulse counting and timing logic** using flip-flops and logic gates
* ⚡ **Analog-to-digital conversion** of heart pulses using comparator circuits
* 🔌 **Completely hardware-based** design with no software or programming
* 🧪 **Educational tool** to learn about biomedical sensing and digital circuit design
  
![project](https://github.com/user-attachments/assets/24c47aa0-be8c-4502-b5c4-ec1395962bcb)



### 🎯 Learning Objectives

This project is ideal for electronics students and enthusiasts interested in:

* Applying **digital counters**, **timers**, and **multiplexing techniques**
* Understanding **biomedical signal acquisition** without microcontrollers
* Building fully hardware-based solutions using discrete logic components
* Exploring **medical electronics** through a practical and hands-on approach

### 📚 Applications

Although simple, this type of digital heart rate monitor has relevance in:

* **Educational demonstrations** and academic labs
* **Low-cost prototype development** in rural or resource-limited settings
* **Basic biomedical instrumentation** without the use of programmable devices


### ⚠️ Limitations

This is a basic implementation and not suitable for clinical diagnosis. It serves purely as an educational prototype. Signal noise, motion artifacts, and accuracy limitations are expected due to the absence of digital filtering or adaptive algorithms.

---

### 👨‍🔧 Contribution

Contributions are welcome to optimize logic design, improve display interfacing, or explore other biomedical signal applications using pure digital logic.
