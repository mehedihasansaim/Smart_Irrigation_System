# 🌱 Smart Irrigation System

## 📌 Project Overview

This project is a **Smart Irrigation System** that automates the watering process based on soil moisture and weather conditions. It helps save water, reduces human effort, and ensures crops get the right amount of water.
The project was implemented using **ESP32**, different sensors, a water pump, and the **Blynk IoT platform**.

---

## 🛠️ Components Used

* **ESP32 Microcontroller**
* **Soil Moisture Sensor** – To measure soil condition
* **Rain Sensor** – To detect rainfall
* **DHT22 Sensor** – For temperature & humidity (optional)
* **Relay Module** – To control the water pump
* **Water Pump**
* **Blynk IoT App** – For remote monitoring and control

---

## ⚡ Circuit Connections

1. Soil Moisture Sensor → ESP32 (Analog pin)
2. Rain Sensor → ESP32 (Digital pin)
3. Relay Module → ESP32 (Digital pin)
4. Relay output → Water Pump
5. ESP32 connected to WiFi → Blynk IoT app

---

## 💻 Software & Libraries

* **Arduino IDE** (for programming ESP32)
* **Libraries Used**:

  * WiFi.h
  * BlynkSimpleEsp32.h
  * DHT.h (if using DHT22)

---

## 🔄 Project Working Procedure

1. **Sensor Data Collection**

   * Soil Moisture sensor checks the dryness level of the soil.
   * Rain Sensor detects whether it is raining.
   * (Optional) DHT22 monitors temperature & humidity.

2. **Data Processing with ESP32**

   * ESP32 reads sensor values.
   * Sends real-time data to the **Blynk Dashboard**.

3. **Decision Making**

   * If soil is dry **AND** no rain → Relay turns **ON** → Pump starts watering.
   * If soil is wet **OR** rain is detected → Pump remains **OFF**.

4. **Remote Monitoring (Blynk App)**

   * Soil & Rain status shown on dashboard.
   * Manual ON/OFF control of water pump possible.
   * Notification alert for rainfall event.

5. **Final Testing**

   * Connected all components on breadboard.
   * Tested in small plant pot.
   * Verified real-time soil condition & pump operation from Blynk app.

---

## 🎥 Project Demonstration

* **Images Folder** → Contains setup pictures.
* **Video File** → Shows live working demo of Smart Irrigation System.

---

## ✅ Results & Benefits

* Saves water by avoiding unnecessary irrigation.
* Reduces manual effort for farmers/gardeners.
* Provides remote monitoring & control from mobile app.
* Scalable for larger agricultural fields.

---

## 🚀 Future Improvements

* Add **fertilizer monitoring system**.
* Use **solar panel** to power the pump.
* Weather forecast integration for smarter irrigation.

---

## 📜 Author

👤 **Mehedi Hasan Saim**

