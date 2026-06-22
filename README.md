# Countdown-timer-for-a-light-system-
# 10-Second Countdown Traffic Light Controller

A digital logic design and simulation of a 10-second countdown traffic light controller system built using **Logisim**. The system counts down from 9 to 0 upon a switch trigger and controls a Red-Amber-Green (RAG) light system based on specific time intervals, displaying the countdown on a 7-segment display.

---

## 📋 Project Specifications & Logic

The system operates based on a 1Hz clock signal and executes the following state transitions:

1. **Idle State:** The system waits for an input button/switch to be pressed.
2. **Start Sequence:** Once pressed, the countdown begins from **9 down to 0**.
3. **Traffic Light Logic:**
   * **At 9 to 8:** Green light is turned **ON** (Amber and Red are OFF).
   * **At 7:** Red light turns **ON**, Amber turns **OFF**.
   * **At 2:** Amber light turns **ON**, Red light turns **OFF**.
   * **At 0:** Green light turns **ON**, Amber turns **OFF**.

---

## 🛠️ Hardware & Component Implementation

The circuit simulates real-world digital ICs and components within Logisim:

* **555 Timer Implementation:** Configured to generate a stable **1Hz clock signal** with a **50% duty cycle** to drive the countdown accurately every second.
* **74193 Counter IC:** Utilized in **down-counting mode** to handle the 4-bit binary countdown sequence from $1001_2$ (9) to $0000_2$ (0).
* **7447 BCD to 7-Segment Decoder:** Converts the 4-bit binary output from the 74193 counter into the corresponding signals to drive a standard **7-Segment Display**.
* **Combinational Logic:** Custom logic gates implemented to decode specific counter states ($7, 2, 0$) and handle the precise switching matrix for the Red, Amber, and Green LEDs.

---

## 📊 Evaluation Criteria Met

This project was built adhering to strict engineering and simulation design standards:
* **Accurate 555 Clock Generation** (1Hz timing)
* **Precise Counter & Down-Counting Logic** (No race conditions)
* **Flawless Traffic Light Truth-Table Logic Implementation**
* **Clean, Modular, and Neat Circuit Layout** in Logisim

---
<img width="1918" height="995" alt="1" src="https://github.com/user-attachments/assets/a8850714-6300-450c-9fbc-cfc77764d88f" />
<img width="1918" height="996" alt="0" src="https://github.com/user-attachments/assets/f2dcc7ec-5706-496d-8a8a-6c4195230c6b" />

2. **Clone the Repository:**
```bash
   git clone [https://github.com/YOUR_GITHUB_USERNAME/traffic-light-countdown-timer.git](https://github.com/YOUR_GITHUB_USERNAME/traffic-light-countdown-timer.git)
