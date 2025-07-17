# Can Satellite PCB Design

This repository contains the PCB design files and documentation for a Can Satellite, featuring multiple environmental and orientation sensors, power management, and wireless communication capabilities. The board is designed for compactness and reliability, suitable for satellite and high-altitude balloon missions.

---

## Sensors Integrated

- **BMP280**: Pressure and temperature sensor  
- **MPU6050**: Accelerometer and gyroscope  
- **LM35**: Analog temperature sensor  
- **MQ135**: Air quality/gas sensor  
- **DHT11**: Temperature and humidity sensor  

## Key Components

- **ESP32**  
  - Handles main processing  
  - Supports I2C and SPI communication for peripherals  
- **TP4056 Charging Module**  
  - Li-ion battery charging management  
- **AMS1117**  
  - 3.3V voltage regulator  
- **LoRa SX1278**  
  - Long-range wireless communication module  

---

## PCB Design Details

- **Track Widths**  
  - **5V Supply:** 0.5 mm  
  - **3.3V Supply:** 0.3 mm  
  - **Signal Traces:** 0.2 mm  

- **Layer Stackup**
  - **Top Layer:** Signals and GND  
  - **First Inner Layer:** GND plane  
  - **Second Inner Layer:** Power plane  
  - **Bottom Layer:** Signals and 5V pad  

---

## Power Management

- **Input:** Li-ion battery (managed by TP4056)
- **Regulation:** AMS1117 provides 3.3V for logic and sensors
- **Separate power and ground planes** for noise reduction and stable operation

---

## Communication

- **LoRa SX1278** for long-range, low-power wireless data transmission
- **ESP32** serves as the central controller, interfacing with sensors and modules via I2C/SPI

---

## Notes

- Carefully matched track widths for power and signal integrity
- Dedicated inner layers for ground and power to minimize noise
- Suitable for CubeSat, CanSat, and other small satellite or experimental payloads

## Photos
<img width="693" height="817" alt="image" src="https://github.com/user-attachments/assets/e986be45-0f04-4dc2-97ea-e7dea023d45b" />
<img width="666" height="817" alt="image" src="https://github.com/user-attachments/assets/16119886-9e38-499b-9a23-71e7e7d9d074" />



