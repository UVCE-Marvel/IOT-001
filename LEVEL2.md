

# **Level 2 – Smart Living & Environmental Automation**


## **Task 1 – Smart Irrigation System**

**Objective:**
Automate plant watering based on soil moisture levels.

**Description:**
Design a smart irrigation system using an ESP32 and a solenoid valve that waters the plant when the soil moisture content goes below a certain threshold.
The system should use a relay to control the valve.

**Requirements:**

* Monitor soil moisture continuously.
* Trigger the solenoid valve using a relay when moisture falls below the set threshold.

**Resource:**
 [How to Control Solenoid Valve Using Arduino](https://circuitdigest.com/microcontroller-projects/how-to-control-solenoid-valve-using-arduino)

**Takeaway:**
Learn automated irrigation using relays and solenoid valves with ESP32.


## **Task 2 – Smart Parking System**

**Objective:**
Monitor parking space availability using ultrasonic sensors.

**Description:**
Develop a smart parking system using an ESP32 and an ultrasonic sensor, integrating it with any IoT platform (e.g., **Blynk**, **Rainmaker**) to detect whether a car is parked in a spot.

**Requirements:**

* Ultrasonic sensor should detect vehicle presence.
* Status should be displayed on the Blynk app.

**Resource:**
[Smart Parking System with Ultrasonic Sensor and Blynk](https://www.youtube.com/watch?v=4LVirWqHk6w&ab_channel=JustDoElectronics)

**Takeaway:**
Learn real-time monitoring and IoT integration using the Blynk platform.



## **Task 3 – Smart Street Lighting with Node-RED Dashboard**

**Objective:**
Create a Smart Street Lighting System and get real-time operational data using a Node-RED dashboard.

**Description:**
Develop an automated street lighting system that uses:

* **LDR sensor** to detect daylight levels.
* **PIR sensor** to sense pedestrian motion.
  The system dims lights during idle periods and brightens them upon motion detection using a relay switch.
  Additionally, send real-time operational data to a **Node-RED dashboard** for monitoring and alerts.

**Requirements:**

* Implement an intelligent street lighting system using an ESP32.
* Use an LDR sensor to detect ambient light levels.
* Use a PIR sensor to detect pedestrian or vehicle motion.
* Dim the street light during idle/dark conditions and brighten upon motion detection.
* Control the lighting system using a relay module.
* Visualize real-time sensor data and system state on a Node-RED Dashboard.

**Resources:**
 [Interfacing with LDR and ESP32](https://www.prateeks.in/2022/09/esp32-interfacing-with-ldr-sensor.html)
 [Interfacing Node-Red with ESP32](https://www.youtube.com/watch?v=wykB7DWI9GM)

**Takeaway:**
Learn how to integrate sensor fusion (LDR + PIR), automate actuation (Relay), and visualize smart infrastructure status using a live Node-RED dashboard.
This task enhances understanding of real-time control systems and IoT-based urban infrastructure.



# **Identification & Cloud Logging**


## **Task 4 – Intro to RFID and Attendance Logger**

**Objective:**
Understand RFID technology and learn to log data on cloud platforms.

### **Part i – Introduction to RFID**

* Learn about RFID cards and RFID card readers.
* Interface an RFID reader with ESP32 and read a metro card.
* Display the card's hex code on the serial monitor.

**Resource:**
 [ESP32 with RFID Access Control](https://www.instructables.com/ESP32-With-RFID-Access-Control/)



### **Part ii – Attendance Logger**

* Use RFID cards to log attendance.
* Display attendance with timestamps on **Google Sheets** using Google App Scripts or any other preferred method.

**Resource:**
 [Attendance Logger with RFID and Google Sheets](https://www.youtube.com/watch?v=ac5CR_bBg74&t=430s&ab_channel=AslamHossain)

**Takeaway:**
Understand RFID technology and learn to log data on cloud platforms.



# **Security & Computer Vision**



## **Task 5 – House Security System**

**Objective:**
Create a security system to detect motion, capture intruder images, and trigger an alert.

**Description:**
Develop a house security system using:

* **ESP32-CAM**
* **PIR motion sensor**
* **Buzzer**, integrated with the **Blynk app**.

**Requirements:**

* PIR sensor to detect motion.
* ESP32-CAM to capture intruder images.
* Buzzer to sound an alarm upon intrusion detection.
* Integrate with Blynk app for real-time alerts and image viewing.

**Resource:**
 [ESP32-CAM Security System](https://www.youtube.com/watch?v=LqX9EMFSoDA&t=164s&ab_channel=TechStudyCell)

**Takeaway:**
Learn home security automation with image capturing and IoT alert systems.



## **Task 6 – Red Light Green Light Game (Squid Game)**

**Objective:**
Build a motion detection game using image processing and sound effects.

**Description:**
Create a **“Red Light Green Light”** game inspired by *Squid Game* using ESP32-CAM, an image recognition model (e.g., OpenCV), and a buzzer.

**Requirements:**

* ESP32-CAM to detect player movements.
* Image recognition model (OpenCV) to identify player movements.
* Use a buzzer to play a sound when a player is eliminated.

**Resources:**
 [Motion Detection with ESP32-CAM](https://how2electronics.com/motion-detection-squid-game-using-esp32-cam-opencv/)
 [Squid Game Red Light Green Light](https://www.youtube.com/watch?v=J7FqiKJmwEI&ab_channel=Danminivlogs)

**Takeaway:**
Learn computer vision, image recognition, and sound integration with ESP32.



# **AI & Voice-Controlled Automation**



## **Task 7 – Creating Your Own Home Assistant**

**Objective:**
Implement voice-controlled home automation.

**Description:**
Build a smart home system using an ESP32 and a microphone sensor, integrated with **ChatGPT** or any **AI model** to control devices using voice commands.

**Requirements:**

* Use a microphone sensor to capture voice commands.
* Control LEDs and motors using ChatGPT or any AI for processing commands.
* Enable question-answer functionality via ChatGPT or AI integration.

**Resources:**
 [ESP32 Voice Recognition](https://www.youtube.com/watch?v=re-dSV_a0tM&t=967s&ab_channel=atomic14)
 [Integrating AI with Home Automation](https://www.youtube.com/watch?v=FZelaG50HEI&ab_channel=BarsAE20)

**Takeaway:**
Learn voice recognition, IoT automation, and AI integration.


