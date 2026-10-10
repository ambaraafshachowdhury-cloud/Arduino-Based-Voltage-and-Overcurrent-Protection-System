# Arduino-Based Voltage & Overcurrent Protection System

## Project Overview
This project is a simulation of a microcontroller-based voltage protector designed to disconnect a load during overvoltage, undervoltage, or overcurrent events. It features local push-button control and serial communication for configuration.

## Repository Structure
- `src/` : Contains the Arduino firmware source code.
- `design_document.pdf` : One-page design report.
- `schematics/` : Proteus schematic and block diagram.
- `test_evidence/` : Screenshots and logs of the simulation testing.
- `project_files/` : Contains the Proteus simulation project files.
- `readme.md` : This file.

## How to Run the Simulation

1. **Download the Project Files:** 
   Download the `project_files.zip` archive from the `project_files/` directory of this repository. 
   *Note: The Arduino `.ino` source code is also included inside this same zip file for your convenience.*

2. **Extract the Zip:** 
   Extract the contents of the zip file to a folder on your computer. You should see a `.pdsprj` file (Proteus Project) and the Arduino code folder.

3. **Open the Simulation:**
   - Launch Proteus Design Suite (Version 8.0 or higher is recommended).
   - Open the `.pdsprj` file.

4. **Load the Firmware:**
   - Open the Arduino code (`.ino` file) from the extracted folder in the Arduino IDE.
   - Compile the code to generate a `.hex` file (or use the `.hex` file already provided in the folder if available).
   - In Proteus, double-click the Arduino Uno component.
   - In the "Program File" field, browse and select the `.hex` file you just compiled.
   - Set the clock frequency to `16MHz`.

5. **Run the Simulation:**
   - Click the "Play" button in Proteus.
   - **Local Control:** Use the push buttons (UP, DOWN, SET, RUN) to navigate the menu and adjust thresholds.
   - **Serial Communication:** Open the Virtual Terminal in Proteus (or use a serial monitor tool) to send commands and view live voltage/current readings. Ensure the baud rate matches the one defined in the code (usually 9600).

## Important Safety Notice
**DO NOT** connect this simulated circuit to actual mains voltage or a real appliance. This is an assessment prototype designed for low-voltage simulation only. Real-world deployment requires proper isolation, calibrated sensors, and electrical safety certification.
