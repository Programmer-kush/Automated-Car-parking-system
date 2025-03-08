# IoT-Based Smart Parking System

## Overview
The **IoT-Based Smart Parking System** is an intelligent and automated parking solution that leverages **YOLOv8** for vehicle detection, **ultrasonic sensors** for slot availability tracking, and **ESP32** microcontrollers for IoT-based communication. This project aims to enhance the efficiency of parking management by minimizing human intervention and ensuring seamless vehicle entry and exit.

## Features
- **Real-time Vehicle Detection**: Uses YOLOv8 to identify incoming vehicles and capture license plates via OCR.
- **Automated Parking Management**: Determines parking slot availability using ultrasonic sensors.
- **Smart Entry & Exit Control**: If a parking slot is available, the system opens the gate automatically.
- **Cloud-Based Data Storage**: Stores vehicle entry and exit details in a database.
- **Live Slot Display**: An LCD screen at the entrance shows real-time slot availability.
- **IoT Communication**: Uses ESP32 to communicate with the cloud via Flask and ThingSpeak.

## System Workflow
1. **Vehicle Detection**: The YOLOv8 model detects an approaching object. If it is classified as a vehicle, the system proceeds to the next step.
2. **License Plate Recognition**: The system captures the vehicle's number plate using OCR and stores it in a cloud database.
3. **Slot Availability Check**: The ESP32 receives a signal to check available parking slots using ultrasonic sensors.
4. **Gate Control**: If a slot is available, the gate opens automatically, allowing the vehicle to enter.
5. **Slot Display**: An LCD near the entrance displays the available slot number or a "No Space Available" message.
6. **Exit Processing**: The system re-detects the vehicle at the exit, logs the exit time, and opens the gate.

## Technologies Used
- **Machine Learning**: YOLOv8 for vehicle detection and OCR for license plate recognition.
- **IoT Hardware**: ESP32 microcontroller, ultrasonic sensors, LCD display.
- **Cloud & Networking**: Flask server for data transmission, ThingSpeak for cloud communication.
- **Database**: Cloud-based storage for tracking vehicle entries and exits.

## My Contributions
- **IoT System Design**: Designed the **IoT architecture and layout**, ensuring smooth integration between hardware and software components.
- **ThingSpeak Communication**: Managed **data transmission between ESP32 and the cloud**, enabling real-time updates on slot availability and gate control.

## Installation & Setup
1. Clone the repository:
   ```bash
   git clone https://github.com/yourusername/smart-parking-system.git
   ```
2. Install dependencies:
   ```bash
   pip install flask opencv-python numpy
   ```
3. Configure ESP32 to connect with the Flask server and ThingSpeak.
4. Train the YOLOv8 model for vehicle detection if needed.
5. Deploy the system and connect all IoT components.

## Future Improvements
- **Integration with Payment Systems** for automated billing.
- **Enhanced AI Models** for improved vehicle detection and plate recognition.
- **Mobile App** for real-time parking status updates and reservations.

- ## Project Report  
You can read the full project report [here](./IOT based Car Parking System.pdf).


---
**Feel free to contribute to this project by submitting pull requests or opening issues!** 🚀

