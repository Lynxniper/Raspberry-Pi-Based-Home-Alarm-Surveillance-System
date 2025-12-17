# Raspberry-Pi-Based-Home-Alarm-Surveillance-System

Overview:
This project implements a cost-effective, real-time security and surveillance system using a Raspberry Pi 4. The system integrates motion detection, video recording, gas/smoke detection, local alarms, and instant mobile notifications to enhance safety in residential and small commercial environments. 

Problem Statement:
Conventional security systems are often expensive, inflexible, and lack real-time responsiveness. Homes and small businesses require an affordable solution that can provide immediate alerts, visual evidence, and hazard detection without complex infrastructure.
This project addresses these challenges by combining multiple sensors and alert mechanisms into a single embedded system controlled by a Raspberry Pi. 

System Features:
1. Motion Detection: PIR sensor detects human movement
2. Video Surveillance: Raspberry Pi camera records video upon motion detection
3. Gas / Smoke Detection: MQ-2 sensor detects smoke and combustible gases
4. Alarm System: LED and buzzer provide visual and audible alerts
5. Real-Time Notifications: Push notifications sent to the user’s mobile device
6. Standalone Operation: Operates locally without cloud dependency

Hardware Components:
1. Raspberry Pi 4
2. PIR Motion Sensor
3. MQ-2 Gas / Smoke Sensor
4. Raspberry Pi Camera Module
5. MCP3008 ADC (for analog sensor input)
6. LED and Buzzer
7. Breadboard and jumper wires
8. 5V Power Supply

System Architecture:
1. The Raspberry Pi acts as the central controller, continuously monitoring sensor inputs:
a. Digital input from PIR sensor for motion detection
b. Analog input from MQ-2 sensor via MCP3008 ADC
c. Trigger-based video recording using the Pi camera
d. GPIO-controlled alarms and notifications
2. Software Stack:
a. Programming Language: Python
b. Libraries:
    RPi.GPIO
    spidev (SPI communication for ADC)
    libcamera (video capture)
    Notification Service: Pushbullet API
c. OS: Raspberry Pi OS

Working Principle:
1. PIR sensor detects motion and triggers the system
2. Camera records video footage of the event
3. MQ-2 sensor monitors gas/smoke levels via ADC
4. If thresholds are exceeded:
5. LED and buzzer are activated
6. Mobile notification is sent instantly
7. System resets and continues monitoring
This ensures rapid response to both security breaches and fire hazards. 

Results:
1. Reliable motion detection with accurate video capture
2. Effective smoke/gas detection based on ppm thresholds
3. Immediate visual, audible, and mobile alerts
4. Stable performance with minimal response delay

Future Enhancements:
1. Face recognition–based intruder identification
2. Rotating camera with servo motor control
3. Remote monitoring dashboard
4. Database-backed event logging
5. Multi-node deployment using wireless modules

Academic Context:
This project was developed as part of the Robotics and Automation (ECE3002B) course under the Department of Electrical and Electronics Engineering.
