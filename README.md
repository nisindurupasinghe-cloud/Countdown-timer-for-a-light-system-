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

---<img width="1918" height="995" alt="9" src="https://github.com/user-attachments/assets/645b118d-01ff-49ba-9df5-cefb15e881ba" />
<img width="1918" height="998" alt="8" src="https://github.com/user-attachments/assets/376ed7e5-b79c-4e0f-83aa-d0bb671872d6" />
<img width="1918" height="952" alt="7" src="https://github.com/user-attachments/assets/4d943055-9d80-4c54-965d-aedb41a887d5" />
<img width="1918" height="995" alt="6" src="https://github.com/user-attachments/assets/b7c2ffbd-b086-4fa2-b5e5-25882ba6dc41" />
<img width="1918" height="995" alt="5" src="https://github.com/user-attachments/assets/521006bd-faf3-4db3-9280-a53fb59adcc7" />
<img width="1918" height="988" alt="4" src="https://github.com/user-attachments/assets/35d835b2-f39e-47a6-aacb-7688ef6aabf7" />
<img width="1918" height="952" alt="3" src="https://github.com/user-attachments/assets/320e01b4-9cb4-44c7-880c-d00990dbcae9" />
<img width="1918" height="992" alt="2" src="https://github.com/user-attachments/assets/8790a674-9b9a-4a27-a568-a5354b82bf54" />
<img width="1918" height="995" alt="1" src="https://github.com/user-attachments/assets/f0b5e724-0aad-4ab5-8ec3-02a5917e3626" />
<img width="1918" height="996" alt="0" src="https://github.com/user-attachments/assets/9079665b-24d4-4166-84a7-2d121001fd0b" />














```bash
   git clone [https://github.com/YOUR_GITHUB_USERNAME/traffic-light-countdown-timer.git](https://github.com/YOUR_GITHUB_USERNAME/traffic-light-countdown-timer.git)
