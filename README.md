## 💓 Heart Rate Monitor – Pure Digital Logic Implementation

This project demonstrates a **heart rate monitoring system** built **entirely using digital electronics components** such as logic gates, flip-flops, comparators, and 7-segment display ICs — with **no microcontroller, Arduino, Raspberry Pi, or programmable logic** involved. It showcases how fundamental principles of digital electronics can be applied to create a functional and educational biomedical device.

### 🧠 Project Overview

The Heart Rate Monitor works by detecting the user's heartbeat using a basic **infrared-based photoplethysmography (PPG) technique**. Blood flow changes in the fingertip cause variations in light absorption, which are captured as analog pulses. These pulses are processed through comparators and converted into clean digital signals.

Using only **digital logic ICs**, the system counts the number of heartbeats in a fixed time interval and then calculates the **beats per minute (BPM)**. The resulting BPM value is displayed using **7-segment displays** to give a real-time readout of the user’s heart rate.

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
