Radar Detection System
This repository contains the complete software and resources for a radar-based detection system. The project uses an ESP32 microcontroller, an ultrasonic sensor (HC-SR04), and a servo motor (SG90) to scan for objects in a 180° arc and display detections on a real-time graphical radar interface.

Project Structure
The repository is divided into the following key sections:

1. Arduino Sensor Code
Platform: ESP32 (Arduino IDE)

Function: Controls the SG90 servo motor to sweep across a 180° range and back.

Sensor Integration: Uses the HC-SR04 ultrasonic sensor to measure the distance of objects at various angles during the sweep.

Output: Sends angle and distance measurements for radar visualization.

Note: Includes embedded WiFi connection code to transmit data over a network.

2. WiFi Connection Code (Standalone Test)
Purpose: Verifies WiFi connectivity of the ESP32 module.

Usage: Provided separately to test and debug network issues.

Note: This functionality is already integrated into the Arduino Sensor Code but is available here for standalone testing.

3. Radar GUI Code
Function: Implements a radar-like graphical user interface (GUI) on a computer.

Features:

Displays real-time angle and distance of detected objects.

Calibrated to visually represent object positions accurately.

Language/Framework: [Specify language used, e.g., Python + Tkinter/Processing/etc.]

4. CAD Files
Contents: 3D model of the sensor housing used to mount the servo and ultrasonic sensor.

Format: [Specify format, e.g., .STL, .F3D, etc.]

Purpose: Provides mechanical design support for physical assembly.

🛠️ Hardware Used
ESP32 Dev Board

HC-SR04 Ultrasonic Sensor

SG90 Servo Motor

3D-printed sensor housing (provided CAD)

Getting Started
Upload the Arduino Sensor Code to the ESP32 using the Arduino IDE.

Ensure WiFi credentials are correctly entered in the code.

Run the Radar GUI Code on your PC to visualize detections.

Use the WiFi Test Code if you're experiencing connectivity issues.

3D-print the housing using the provided CAD files for accurate sensor mounting.
