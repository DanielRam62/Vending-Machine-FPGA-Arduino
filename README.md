Automatic Vending Machine using FPGA & Arduino
Project Overview
This project demonstrates the integration of FPGA (Basys3) and Arduino Uno to implement an automatic vending machine with real-time user interaction. The system allows users to select a product, insert coins, and receive change, utilizing a combination of hardware logic, embedded programming, and serial communication.

The vending machine operates using:

FPGA (Basys3) – Handles product selection, payment validation, and change calculation.
Arduino Uno – Manages LCD display, user inputs (buttons), and serial communication with the FPGA.
UART Communication – Ensures reliable data exchange between FPGA and Arduino.
LCD Display & 7-Segment Display – Provide real-time feedback to the user.
This project is ideal for embedded systems enthusiasts, FPGA developers, and engineering students looking to understand hardware-software co-design.

Features
✅ Real-time User Interface – LCD shows product selection, inserted amount, and transaction status.
✅ FPGA-Based Processing – Ensures high-speed calculations for product pricing and change distribution.
✅ Efficient Coin Handling – Tracks available coins and dispenses optimal change.
✅ Multiplexed 7-Segment Display – Displays product codes and transaction details.
✅ Admin Mode – Monitors total earnings and available coin stock.

System Architecture
The system consists of two primary components:

1. FPGA (Basys3) - Digital Controller
Manages product selection and pricing.
Receives inserted coin values from Arduino.
Calculates change and determines optimal coin distribution.
Controls 7-segment display for numerical output.
Communicates with Arduino over UART.
2. Arduino Uno - User Interface & Payment Handling
Reads user inputs from buttons (coin insertion & confirmation).
Displays messages on LCD (product info, inserted amount, transaction status).
Sends coin data to FPGA for processing.
Receives processed information (product price, change calculation).
Provides an admin mode to monitor total earnings and coin stock.
Hardware Components
🟢 Basys3 FPGA Board (Xilinx Artix-7)
🟢 Arduino Uno (ATmega328P)
🟢 16x2 LCD Display (I2C communication)
🟢 7-Segment Display (Common Anode)
🟢 Push Buttons (Coin input, product selection, admin mode)
🟢 Resistors & Wires (Breadboard-based connections)

Software & Tools
💻 Vivado Design Suite – FPGA Design & Simulation
💻 Arduino IDE – Microcontroller Programming
💻 ModelSim/QuestaSim – Verilog Simulation
💻 GitHub – Version Control & Documentation

Installation & Setup
1. Clone the Repository
bash
Copy
Edit
git clone https://github.com/yourusername/VendingMachine-FPGA-Arduino.git
cd VendingMachine-FPGA-Arduino
2. Hardware Setup
Connect Arduino to FPGA using defined UART pins.
Wire push buttons for coin insertion and selection.
Ensure LCD and 7-segment display are properly connected.
3. Upload Arduino Code
Open Arduino IDE.
Upload arduino_vending.ino to the Arduino Uno.
4. Synthesize FPGA Code
Open Vivado.
Import Verilog source files.
Run Synthesis & Bitstream Generation.
Program the Basys3 FPGA.
Demonstration
📹 A detailed video demonstration is included in the media/ folder.
🖼️ Images showcasing the system operation are available in images/.
📄 Project poster and final documentation are available in docs/.

Project Structure
bash
Copy
Edit
📂 VendingMachine-FPGA-Arduino
│── 📂 src                # Source code (Verilog & Arduino)
│── 📂 images             # System setup and demo images
│── 📂 docs               # Project documentation, reports, and presentation
│── 📂 media              # Video demonstrations
│── 📄 README.md          # Project description
│── 📄 LICENSE            # Open-source license
Future Improvements
🔹 RFID/NFC Payment – Allow cashless payments via RFID/NFC.
🔹 Touchscreen Interface – Replace buttons with an interactive touchscreen.
🔹 Expanded Product Selection – Increase supported products beyond basic pharmaceuticals.

Contributors
👨‍💻 Daniel Ram – FPGA & Hardware Engineer

For inquiries or contributions, feel free to reach out via GitHub Issues or email.

License
This project is open-source and licensed under the MIT License.

