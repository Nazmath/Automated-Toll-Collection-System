# 🚗 Automated Toll Collection System using Arduino & RFID

This project demonstrates an **Automated Toll Collection System** built using **Arduino Uno** and an **RFID module (RC522)**.  
The system scans RFID cards to identify registered vehicles, automatically opens a gate using a servo motor, and closes it after a short delay.  
It is a beginner-friendly IoT/embedded project that can be extended for real-world applications like smart toll booths.

---

## 📜 Table of Contents
- [Features](#-features)
- [Components Used](#-components-used)
- [Circuit Diagram](#-circuit-diagram)
- [Working Principle](#-working-principle)
- [How to Run](#-how-to-run)
- [Future Enhancements](#-future-enhancements)
- [License](#-license)

---

## ✨ Features
✔ RFID-based vehicle identification  
✔ Automatic toll gate operation using servo motor  
✔ Easy configuration of RFID card IDs  
✔ Low-cost, compact, and scalable design  
✔ Optional LCD and buzzer integration for better user feedback  

---

## 🔧 Components Used
| Component              | Quantity |
|------------------------|----------|
| Arduino Uno            | 1        |
| RC522 RFID Module      | 1        |
| RFID Card/Tag          | 1+       |
| Servo Motor            | 1        |
| Jumper Wires           | As needed |
| Breadboard (optional)  | 1        |
| LCD Display (optional) | 1        |
| Buzzer (optional)      | 1        |

---

## 🔌 Circuit Diagram
| RFID RC522 | Arduino Uno |
|------------|-------------|
| SDA (SS)   | D10         |
| SCK        | D13         |
| MOSI       | D11         |
| MISO       | D12         |
| RST        | D9          |
| 3.3V       | 3.3V        |
| GND        | GND         |

| Servo | Arduino |
|-------|----------|
| VCC   | 5V       |
| GND   | GND      |
| Signal| D3       |

*(Insert your circuit diagram image here)*

---

## ⚙️ Working Principle
1. The RFID reader scans the RFID card’s **UID**.  
2. If the UID matches the stored ID, the **servo motor rotates** to open the gate.  
3. After a delay, the servo rotates back to **close the gate**.  
4. Unauthorized cards are rejected, keeping the gate closed.  

---

## ▶️ How to Run
1. **Connect components** as per the wiring diagram.  
2. **Install the MFRC522 library** in Arduino IDE.  
   - Go to: `Sketch → Include Library → Manage Libraries → Search MFRC522 → Install`  
3. **Upload the Arduino code** to your board.  
4. Open Serial Monitor at **9600 baud**.  
5. Scan your RFID card/tag to see the gate in action!  

---

## 🚀 Future Enhancements
- Integration with **online toll payment systems**  
- GSM/WiFi module for **remote monitoring**  
- Storing **transaction logs** on an SD card  
- Multi-lane toll booth implementation  

---

## 📜 License
This project is open-source and free to use for educational purposes.  
Feel free to fork and modify for your needs.  

---

### 👨‍💻 Author
NAZMATH PASHA 
Project for Embedded Systems & IoT learning.  

---
