
# **Level 1 – Introduction to ESP32 & Basic Components**

---

## **Task 1a – Theory: Digital I/O & Interrupts**

**Objective:**
Study GPIO configuration and interrupts for efficient input handling.

**Description:**
Study and comprehend the hardware and software principles behind GPIO pin configuration, including input, output, pull-up/down resistors, and interrupt-driven event handling on the ESP32.
Students will explore how interrupts optimize system responsiveness for button presses without constant polling.

**Resource:** [Pinout of ESP32](https://randomnerdtutorials.com/esp32-pinout-reference-gpios/)

---

## **Task 1b – Simon Says Game using ESP32**

**Objective:**
Familiarize with the ESP32 microcontroller by creating an engaging game.

**Description:**
Create a fun and interactive *Simon Says* game using an ESP32, pushbuttons, and LEDs.
The game should blink the LEDs in a random sequence, and the user needs to press the corresponding buttons in the correct order.
If the user fails, provide a clear indication (e.g., all LEDs flashing) and restart the game.

**Resource:** Modify the existing [Wokwi Simulation](https://wokwi.com/) for ESP32 compatibility.

---

## **Task 2 – Temperature-Based Fan Control**

**Objective:**
Automate fan (DC motor) control using a temperature sensor and relay.

**Description:**
Create an automated temperature regulation system where a DHT11 sensor continuously monitors ambient temperature, displaying readings via the serial monitor.
When temperature crosses a pre-set threshold, the motor driver will signal the DC motor to turn on at the appropriate speed.
This task integrates sensor data acquisition with actuator control to demonstrate real-world environmental automation concepts.

**Resource:** [Temperature Controlled Fan](https://www.youtube.com/watch?v=WDYNgw0EE6o)

---

# **Communication Protocols**

---

## **Task 3a – IoT Communication Protocols**

**Objective:**
Understand IoT and Serial protocols: MQTT, HTTP, I2C, SPI.

**Description:**
Gain theoretical knowledge of common IoT communication protocols (MQTT, CoAP, HTTP, etc.), understanding their characteristics, trade-offs, and suitable use cases.

**Resources:**

* [IoT Communication Protocol](https://www.tutorialspoint.com/cryptography/communication_protocols_for_iot_devices.htm)
* [Serial Communication Protocol](https://circuitdigest.com/tutorial/serial-communication-protocols)

---

## **Task 3b – Controlling LEDs Using MQTT**

**Objective:**
Utilize any MQTT platform to establish publishing and subscribing functionalities.

**Description:**
Explore the basics of the MQTT protocol and its working. Learn about different communication and network protocols.
Upon publishing a message to control LEDs, the subscribers should receive the message and activate the corresponding LED accordingly.

**Example:**

```
LED 1 ON  → Turns on the first LED  
LED 1 OFF → Turns off the first LED  
```

Similarly, control **LED 2** and **LED 3**.

**Resources:**

* [MQTT X Features](https://mqttx.app/features)
* [ESP8266 MQTT LED Control](https://www.emqx.com/en/blog/esp8266_mqtt_led)

**Takeaway:**
Understand MQTT communication and apply it to control hardware remotely.

---

## **Task 4 – Communication using I2C Protocol**

**Objective:**
* Both ESP32 boards should host web servers for bidirectional communication.
* The typed message on one webserver should be displayed on the LCD connected to the other ESP32.

**Description:**
Send data between two ESP32 boards using the I2C protocol.
Display a message on an LCD screen by typing the message using a webserver hosted on the ESP32.

**Takeaway:**
Learn wired communication between two microcontrollers using the I2C protocol.

**Resource:** [ESP32 I2C Master and Slave](https://randomnerdtutorials.com/esp32-i2c-master-slave-arduino/)

---

# **Cloud Communication & Data Logging**

---

## **Task 5 – Sending Data to ThingSpeak and Creating a Regression Model**

**Objective:**

* Publish temperature data from ESP32 to ThingSpeak.
* Retrieve the dataset from ThingSpeak for analysis.
* Using Matplotlib in Python, plot the graph of **Temperature vs. Time**.
* Create a regression model to analyze the relationship between **Humidity (from a DHT11 sensor)** and **Moisture Percentage (from a capacitive soil moisture sensor)**.

**Description:**
Using an ESP32, post temperature data from a sensor and soil moisture data to the ThingSpeak website using its API and display graphs:

* **Temperature vs. Soil Moisture**
* **Humidity vs. Soil Moisture**

Retrieve the data back from ThingSpeak and create a regression model.

**Plot the Regression Graph:**

* **X-axis:** Humidity
* **Y-axis:** Moisture Percentage

**Resources:**

* [Basics of Linear and Logistic Regression](https://hub.uvcemarvel.in/course/AI-ML-001#2)
* [Soil Moisture Monitoring with Arduino and Machine Learning](https://github.com/sohamroy3/Soil-moisture-Monitoring-using-arduino-with-machine-learning)
* [ESP32 HTTP POST with IFTTT and ThingSpeak](https://randomnerdtutorials.com/esp32-http-post-ifttt-thingspeak-arduino/)
* [Send Data to ThingSpeak with Arduino](https://nothans.com/thingspeak-tutorials/arduino/send-data-to-thingspeak-with-arduino)

**Takeaway:**
Learn to publish and retrieve data from a web server, analyze data, and apply machine learning for prediction.

---

# **Web Servers & Local Interfaces**

---

## **Task 6 – Flashing Morse Code**

**Objective:**
Create a website that converts typed input (normal words) to Morse code.
The LED should blink according to the Morse code generated.

**Description:**
Set up an ESP32 to flash Morse code using an LED. The message is sent through a webserver hosted on the ESP32.

**Resource:** [Morse Code with Arduino](https://www.instructables.com/Morse-code-with-arduinoLED/)

**Takeaway:**
Understand the application of webservers in communication.

---

## **Task 7 – Health Vitals Dashboard**

**Objective:**
Plot graphs of the vitals on a webserver for real-time monitoring.

**Description:**
Measure heart rate and blood oxygen levels using the pulse sensor and display the results graphically on a webserver.

**Resources:**

* [Pulse sensor Esp32](https://microcontrollerslab.com/pulse-sensor-esp32-tutorial/)
* [Plot Chart on Web Server](https://randomnerdtutorials.com/esp32-esp8266-plot-chart-web-server/)

**Takeaway:**
Learn to monitor health vitals and display data graphically on a webserver.

---

# **Actuation, Surveillance & Alerts**

---

## **Task 8 – Wi-Fi Controlled Surveillance Bot with Live Video Stream**

**Objective:**
Create a surveillance bot capable of capturing live video feed and remotely controlling its movements.

**Description:**
Build a surveillance robot using an ESP32-CAM and L298N motor driver. Implement live video streaming and enable remote control functionality over Wi-Fi.

**Specific Requirements:**

* Use **L298N Motor Driver** for movement control.
* Set up **live video streaming server**.
* Upload the captured video to the **MARVEL website**.

**Resource:** [ESP32-CAM Surveillance Robot](https://iotdesignpro.com/projects/esp32-cam-surveillance-robot-car)

**Takeaway:**
Learn video streaming, remote control, and motor driver interfacing with ESP32.

---

## **Task 9 – Fire Alarm System with SMS Alerts**

**Objective:**
Learn about fire detection and integrating SMS alert systems using APIs.

**Description:**
Develop a fire alarm system using the ESP32 microcontroller with fire sensors.
On detecting heat, the ESP32 triggers an SMS alert using the **Twilio API** or any other platform.

> ⚠️ **Important:** This task must be tested under supervision due to safety precautions.

**Resources:**

* [ESP32 Flame Sensor](https://esp32io.com/tutorials/esp32-flame-sensor)
* [Sending SMS Alerts with ESP32](https://iotdesignpro.com/articles/sending-sms-alerts-with-esp32-using-twilio)

**Takeaway:**
Learn about fire detection and integrating SMS alert systems using APIs.






