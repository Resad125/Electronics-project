 #  Electronics Engineering - Individual Portfolio
 This repository contains my structured academic portfolio submissions for the Electronics Engineering course. The deliverables follow the required chronological sequence up to the final project integration.

# 🚀 Featured Project: Project 2.6 -Advanced Smart Home and Environmental Control Systems
# Project description 
An integrated, multi-sensor smart home automation and security loop system built with Arduino Uno R3. This project manages automated climate scaling, ambient light tracking, and event-driven emergency intrusion overrides.

### Core Features:
* **Climate Control:** Automated DC Motor fan speed modulation based on TMP36 temperature feedback (> 28°C).
* **Smart Lighting:** Continuous ambient light intensity tracking using an LDR photocell circuit.
* **Intrusion Security:** High-priority visual (LED) and acoustic (Piezo Buzzer) alert system triggered instantly via PIR motion detection.

# Final Deliverables (Academia.edu & YouTube Video)
As per the final portfolio evaluation criteria, the verified technical documentation and the full video explanation are published below:

• 📑 Official Technical Paper (Academia.edu): [Click Here to Read the Full Publication on Academia.edu]
•https://www.academia.edu/167426041/Individual_Project_Portfolio_Project_2_6?source=swp_share

• 🎥 5-Minute Technical Video Presentation (YouTube): [Click Here to Watch the Video Demonstration on YouTube]
https://youtu.be/2tRkW_6PprY?si=vYZFsISPvdJWm3N-

### Circuit Schematic & Simulation Environment

* **Platform:** Autodesk Tinkercad
* **Control Modes:**
  * **Autonomous Smart Mode:** Closed-loop automated processing via continuous polling of TMP36 (temperature) and LDR (light-dependent resistor) feeds.
  * **Safety Priority Override:** Real-time event-driven interrupt logic triggered by the PIR sensor to immediately execute acoustic-visual emergency routines.

# My copybook
https://drive.google.com/file/d/18-HTkukPw251G76OUwly5ij86eXo6s7-/view?usp=drivesdk

# Full Project Description

This system functions as an integrated smart home infrastructure that simultaneously processes environmental data streams and maintains safety protocols through deterministic control logic:

* **Environmental Logic (Continuous Loop):** The micro-controller constantly monitors ambient variables via analog signals. The **TMP36** reads thermal levels, and the code converts raw voltage into Celsius degrees. If the system detects temperature values strictly above **28.0°C**, it triggers the **DC Motor (HVAC simulation)** at an optimized analog PWM duty cycle of 220 to initiate automated cooling. Concurrently, the **LDR circuit** monitors lighting levels and streams live telemetry directly to the visual terminal.
* **Safety & Threat Mitigation Logic:** The system operates with an embedded security override routine. While the LCD normally outputs standard LDR sensor data, the **PIR Motion Sensor** acts as a system trigger. The moment spatial motion changes state to `HIGH`, the firmware immediately interrupts the idle display cycle, prints an explicit **"ALARM! Motion"** alert across the interface, and executes a synchronized acoustic-visual distress routine via the **Piezo Buzzer** and **Red LED**.

---

# Verification & Testing

To verify the system's runtime stability and code correctness, systematic environmental boundary tests were executed within the Autodesk Tinkercad simulation environment:

| Test Case Scenario | Input State / Conditions | Expected System Output | Verification Result |
| :--- | :--- | :--- | :--- |
| **1. Idle Light Tracking** | PIR = `LOW`, Temp = 24.6°C, LDR active | LCD displays current temperature and raw LDR values. DC Motor & Buzzer are completely idle. | **PASSED** |
| **2. Active Climate Cooling** | PIR = `LOW`, Temp = 31.2°C (>28°C) | LCD updates temperature. DC Motor spins at high speed (PWM 220). Alarm remains quiet. | **PASSED** |
| **3. Security Intrusion Alert** | PIR = `HIGH` (Motion Detected) | LCD instantly prints "ALARM! Motion". Piezo Buzzer sounds continuously and Red LED stays fully lit. | **PASSED** |

#### Hardware Stability Controls:
* **Contrast Glitch Protection:** The LCD's `V0` (contrast) and `RW` (Read/Write) pins are securely strapped to the common ground rail (`GND`) to eliminate simulation visual corruption and empty display blocks.
* **Current Limiting:** The Red LED matrix line is isolated using a **220Ω resistor** to prevent simulation overcurrent warnings on the microcontroller output pins.


# Verified by: Telman Askeraliyev (Fizika Müəllimi) – Azerbaijan
Contact: 
# Linkedln: https://www.linkedin.com/in/physics-teacher-azerbaijan-telman-askeraliyev?utm_source=share&utm_campaign=share_via&utm_content=profile&utm_medium=ios_app

# İnstagram: https://www.instagram.com/physics_teacher_azerbaijan?igsh=MW1sa2trcnN3d3B2aw==





# All  Electronics Projects
1.Understanding the capacitor

https://www.slideshare.net/slideshow/ruslan-qasimov-kamran-liquliyev-f-rid-liyev-emin-r-himov-m-sud-n-sirov-r-mzi-huseynli-r-sad-m-mm-dov-pdf/286799768


2.Technical Laboratory Report: Automatic Light Sensing and Voltage Divider Circuit

https://www.academia.edu/165908187/Technical_Laboratory_Report_Automatic_Light_Sensing_and_Voltage_Divider_Circuit_Khanverdi_Chalabiyev_Emin_Rahimov_Resad_Memmedov_Vasif_Sarifzade_Kamran_Aliquliyev_Verified_by_Physics_Teacher_Azerbaijan_Telman_Askeraliyev_Fizika_Muellimi_Azerbaijan_Baku_


3.Azerbaijan's Electronics Sector Challenges

https://www.slideshare.net/slideshow/electronics-sector-gaps-in-azerbaijan-pdf-87a2/287506108


4.Field Effect Transistors

https://www.slideshare.net/slideshow/fet_presentation-pdf-farid-aliyev-masud-nasirov-ramzi-huseynli-rashad-mammadov-tuqay-qarayev/287505953

5.Voltage Regulators

https://www.slideshare.net/slideshow/physics-guide-an-analysis-of-authors-m-sud-n-sirov-f-rid-liyev-tuqay-qarayev-r-mzi-huseynli-r-sad-m-mm-dov-verified-by-physics-teacher-azerbaijan-telman-askeraliyev-fizika-muellimi-azerbaijan-baku/287505357



