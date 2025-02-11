# 🚀 Automatic Vending Machine using FPGA & Arduino

## 📌 Project Overview
This project implements an **automatic vending machine** using **FPGA (Basys3)** and **Arduino Uno**, enabling real-time product selection, payment processing, and change distribution. The system integrates **hardware-software co-design** through **UART communication** between the FPGA and Arduino.

Key Features:
- **Product selection & price display**
- **Real-time coin tracking & optimal change calculation**
- **Admin mode for earnings & coin stock monitoring**
- **LCD and 7-segment display integration**
- **Reliable UART communication between FPGA & Arduino**

---

## 🏗️ System Architecture

### **🖥️ FPGA (Basys3) - Digital Controller**
- Handles **product selection**, **payment validation**, and **change calculation**.
- Controls **7-segment display** for price visualization.
- Communicates with Arduino via **UART**.
- Determines **optimal coin distribution** for change return.

### **📟 Arduino Uno - User Interface & Payment Handling**
- Reads **user inputs** from push buttons.
- Displays transaction details on **LCD screen**.
- Sends **inserted coin data** to FPGA.
- Receives **processed payment & change data** from FPGA.
- Includes **Admin Mode** to monitor coin stock and earnings.

---

## 🛠️ Hardware Components
| Component        | Description |
|-----------------|-------------|
| **Basys3 FPGA** | Xilinx Artix-7 based FPGA for processing transactions |
| **Arduino Uno** | Microcontroller for user interface & UART communication |
| **LCD Display** | 16x2 I2C LCD for transaction information |
| **7-Segment Display** | Multiplexed display for real-time pricing |
| **Push Buttons** | Used for coin insertion and product selection |
| **Resistors & Wires** | Hardware connectivity |

---

## 💻 Software & Tools Used
- **Vivado Design Suite** – FPGA Design & Synthesis
- **Arduino IDE** – Microcontroller Programming
- **ModelSim/QuestaSim** – Verilog Simulation
- **GitHub** – Version Control & Documentation

---

## 🔧 Installation & Setup

### **1️⃣ Clone the Repository**
```bash
git clone https://github.com/yourusername/VendingMachine-FPGA-Arduino.git
cd VendingMachine-FPGA-Arduino

### **2️⃣ Hardware Setup
-Connect Arduino to FPGA via UART.
-Wire push buttons for coin insertion & selection.
-Ensure LCD & 7-segment display are properly connected.

### **3️⃣ Upload Arduino Code
# Open Arduino IDE
# Select Arduino Uno Board
# Upload the arduino_vending.ino file

4️⃣ Synthesize & Load FPGA Code
# Open Vivado
# Import Verilog files
# Run Synthesis & Bitstream Generation
# Program Basys3 FPGA

📸 Demonstration
📹 A video demonstration is included in media/.
🖼️ System images are stored in images/.
📄 The project report, presentation, and poster are available in docs/.

📂 Project Structure
📂 VendingMachine-FPGA-Arduino
│── 📂 src                # Source code (Verilog & Arduino)
│── 📂 images             # System setup and demo images
│── 📂 docs               # Project documentation, reports, and presentation
│── 📂 media              # Video demonstrations
│── 📄 README.md          # Project description
│── 📄 LICENSE            # Open-source license

🚀 Future Improvements
🔹 RFID/NFC Payment Support – Enable cashless transactions.
🔹 Touchscreen Interface – Replace buttons with an interactive UI.
🔹 Expanded Product Catalog – Increase vending machine flexibility.

👨‍💻 Contributors
Name	Role
Your Name	FPGA & Embedded Systems Engineer
📩 Feel free to reach out via GitHub Issues for inquiries or contributions.
