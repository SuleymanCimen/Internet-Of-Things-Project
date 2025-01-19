IoT-Based Collision Detection System Using TinyML

Introduction
This project focuses on developing an Internet of Things (IoT)-based collision detection system using the ESP32 microcontroller, accelerometer (ADXL345), pressure sensor, and GPS module. The system is designed to detect vehicle accidents, classify their severity as either minor or major, and transmit the location coordinates to emergency response teams. The decision-making mechanism leverages TinyML, with a model trained on Edge Impulse, achieving 97% prediction accuracy.

Key Features
Accident Detection:
Utilizes accelerometer and pressure sensor data to identify collision events and classify their severity.
Location Reporting:
GPS module transmits the exact coordinates of the incident to cloud-based systems for emergency response.
Cloud Integration:
AWS IoT Core and CloudWatch are used to store and analyze data, with Grafana providing visualization.
Energy Efficiency:
The system runs on the ESP32 microcontroller with low power consumption, suitable for IoT applications.
Machine Learning Integration:
TinyML model trained on Edge Impulse ensures accurate real-time decision-making.

Hardware Components
ESP32 Microcontroller: Processes sensor data and manages communication with the cloud.
ADXL345 Accelerometer: Captures 3-axis acceleration data to detect collisions.
Pressure Sensor: Measures impact forces to improve classification accuracy.
GPS Module: Determines and transmits location coordinates during an accident.
Software and Machine Learning
TinyML Model:
Trained using Edge Impulse with 208 training samples and 57 test samples.
Achieves 97.6% accuracy in classifying normal driving, minor accidents, and major accidents.
Cloud Integration:
AWS IoT Core and MQTT protocol enable seamless data transmission.
CloudWatch stores logs, and Grafana visualizes accident data on dashboards.

Outcomes
The system effectively detects and classifies collisions with high accuracy. Emergency response teams are promptly notified with precise location data, ensuring timely intervention. The integration of accelerometer and pressure sensors enhances reliability, while the GPS module enables accurate reporting of accident locations.

