# 🚚 Low Budget Automated Dispatch System (STM32 + RFID + LCD)

A cost-effective automated dispatch system using an STM32 microcontroller, RC522 RFID reader, and I2C LCD display. Designed for smart, low-cost applications in logistics, attendance, or resource deployment.

## 💡 Project Overview

This system uses RFID authentication to trigger dispatch events. It can identify users or resources via RFID tags and display their status on an I2C LCD. Built on STM32 for improved performance and cost-efficiency.



## 🔧 Features

- ✅ STM32 microcontroller-based (e.g., STM32F401CCU6)
- ✅ RFID-based dispatch triggering using MFRC522
- ✅ I2C LCD for real-time status display
- ✅ Low power and budget-friendly
- ✅ Scalable for attendance, logistics, or access control systems

## 🧰 Hardware Requirements

- STM32F401CCU6 (Black Pill) or similar STM32 board
- MFRC522 RFID Reader Module
- I2C LCD Display (16x2 or 20x4)
- RFID Tags/Cards (13.56 MHz)
- Optional: Buzzer, Relay Module
- Power Supply (5V regulated)

### 🔌 STM32 Pin Configuration Example

| Component  | Pin        |
|------------|------------|
| MFRC522 SDA | PA4       |
| MFRC522 SCK | PA5       |
| MFRC522 MOSI| PA7       |
| MFRC522 MISO| PA6       |
| MFRC522 RST | PB0       |
| LCD SDA    | PB7       |
| LCD SCL    | PB6       |

> *Pin assignments may vary based on your STM32 board and library.*

## 🧪 Software Requirements

- STM32CubeIDE or PlatformIO
- STM32 HAL or LL drivers
- MFRC522 and I2C LCD libraries
- Open-source RFID and LCD drivers compatible with STM32

## 🛠️ Installation Steps

1. Connect hardware as per the pin configuration above.
2. Install required libraries for RFID and I2C LCD in STM32CubeIDE.
3. Flash the firmware to STM32 using ST-Link or USB.
4. Place RFID tag/card near reader to simulate a dispatch event.
5. LCD displays dispatch status or access confirmation.

## 📊 How It Works

- RFID tag is scanned using the RC522 module.
- STM32 authenticates the tag and logs or triggers a dispatch action.
- LCD displays current status: ID verified, Dispatch started, etc.
- Optional: Relay activates a gate, motor, or signal upon valid dispatch.


---

## 🧠 Applications

- 🏢 **Attendance Systems** — Log employees/students using RFID tags  
- 🚛 **Logistics Dispatch** — Automate dispatch of delivery vehicles or equipment  
- 🚪 **Access Control** — Trigger doors or gates upon RFID verification  
- 🏭 **Industrial Automation** — Assign tasks to machines or lines based on scanned IDs  
- 🚨 **Emergency Response** — Dispatch emergency units by authorized personnel scans  

---

## 📄 License

This project is licensed under the **MIT License**.  
You are free to use, modify, and distribute this code for personal or commercial purposes with proper attribution.

---

*Crafted for embedded enthusiasts and real-world automation, powered by STM32.*


