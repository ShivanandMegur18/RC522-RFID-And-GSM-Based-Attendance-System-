# 📡 RC522 RFID and GSM-Based Attendance System

An Arduino-based attendance management system that uses RFID technology to identify users and GSM communication to send attendance notifications through SMS.

This project demonstrates the practical application of embedded systems, RFID identification, and wireless communication for automated attendance management.

## 🎯 Project Objectives

* Automate the attendance recording process using RFID cards.
* Identify registered users using the RC522 RFID reader.
* Use a GSM module to send attendance notifications via SMS.
* Reduce manual effort in maintaining attendance records.
* Demonstrate embedded systems and serial communication concepts.

## ✨ Features

* 📇 RFID-based user identification.
* ⚡ Automatic attendance detection.
* 📱 GSM-based SMS notifications.
* 🔌 Arduino-based embedded system.
* 🛠️ Expandable design for future enhancements.

## 🧰 Hardware Components

| Sl. No. | Component         | Purpose                                |
| ------- | ----------------- | -------------------------------------- |
| 1       | Arduino board     | Main controller                        |
| 2       | RC522 RFID Reader | Reads RFID card data                   |
| 3       | RFID Cards/Tags   | Identifies registered users            |
| 4       | GSM Module        | Sends SMS notifications                |
| 5       | SIM Card          | Provides cellular network connectivity |
| 6       | Jumper Wires      | Connects the components                |
| 7       | Breadboard        | Supports circuit prototyping           |
| 8       | Power Supply      | Powers the system                      |

**Note:** Update this list to match the actual components used in your implementation.

## 💻 Software Requirements

* Arduino IDE
* Arduino-compatible USB driver
* Required Arduino libraries
* Compatible GSM network and SIM card

## ⚙️ Working Principle

1. The system initializes the Arduino, RFID reader, and GSM module.
2. A user scans an RFID card or tag.
3. The RC522 reader reads the card's unique identifier (UID).
4. The Arduino compares the UID with the registered user records.
5. If the card is authorized, the system records the attendance event.
6. The GSM module sends an SMS notification if the notification feature is configured.
7. Unauthorized cards can be rejected by the system.

**Note:** The actual behavior depends on the features implemented in the Arduino program.

## 🔌 Circuit Connections

Connect the RC522 RFID reader and GSM module to the Arduino according to the interfaces supported by your specific hardware.

### RC522 RFID Reader

The RC522 commonly communicates with Arduino through SPI.

| RC522 Pin | Arduino Connection                  |
| --------- | ----------------------------------- |
| SDA / SS  | Configured SPI chip-select pin      |
| SCK       | SPI clock pin                       |
| MOSI      | SPI MOSI pin                        |
| MISO      | SPI MISO pin                        |
| IRQ       | Optional; depends on implementation |
| GND       | GND                                 |
| RST       | Configured reset pin                |
| 3.3V      | 3.3V supply                         |

**Important:** The RC522 operates at 3.3 V. Do not connect its power pin to 5 V. Check voltage compatibility between the RC522 and your Arduino board's signal pins.

The GSM module's connections depend on the specific model and Arduino board. Refer to the module's datasheet for power, UART, and logic-level requirements.

## 🚀 Getting Started

### 1. Clone the Repository

```bash
git clone https://github.com/ShivanandMegur18/RC522-RFID-And-GSM-Based-Attendance-System-.git
```

### 2. Open the Project

Navigate to the project directory:

```bash
cd rfid-gsm-attendance-system
```

Open the Arduino sketch located at:

```text
src/attendance_system.ino
```

### 3. Install Required Libraries

Open Arduino IDE and install the libraries required by your sketch.

For example, if your code uses the MFRC522 library, install the appropriate library through the Arduino IDE Library Manager.

### 4. Configure the Hardware

* Connect the RC522 RFID reader.
* Connect the GSM module.
* Insert a compatible SIM card into the GSM module.
* Verify all power and signal connections.
* Configure the pins in the source code to match your circuit.

### 5. Upload the Code

1. Connect the Arduino to your computer.
2. Select the correct board in Arduino IDE.
3. Select the correct serial port.
4. Compile and upload the sketch.
5. Open Serial Monitor to check the system status.

### 6. Test the System

* Scan a registered RFID card.
* Check whether the card is identified correctly.
* Verify the attendance behavior implemented in the sketch.
* Check whether the GSM module sends the configured SMS notification.

## 📂 Repository Structure

```text
rfid-gsm-attendance-system/
│
├── README.md
├── LICENSE
├── .gitignore
│
├── src/
│   └── attendance_system.ino
│
├── docs/
│   └── circuit_diagram.png
│
├── images/
│   └── project_setup.jpg
│
└── examples/
    └── rfid_test.ino
```

## 🔮 Future Enhancements

* Store attendance records in a database.
* Add an LCD or OLED display.
* Implement date and time tracking using an RTC module.
* Generate daily and monthly attendance reports.
* Integrate Wi-Fi or IoT-based attendance monitoring.
* Develop a web dashboard for attendance management.

## 🎓 Applications

* Schools and colleges
* Office attendance management
* Laboratory access monitoring
* Employee attendance systems
* Embedded systems learning projects

## 📚 Concepts Demonstrated

* Embedded C/C++ programming
* SPI communication
* UART serial communication
* RFID identification
* GSM-based wireless communication
* Hardware interfacing
* Microcontroller-based system design

## 📜 License

This project is licensed under the MIT License. See the [LICENSE](LICENSE) file for details.

## 👨‍💻 Author

**Shivanand Basavaraj Megur**

Electronics and Communication Engineering

GitHub: [@ShivanandMegur18](https://github.com/ShivanandMegur18/RC522-RFID-And-GSM-Based-Attendance-System-.git)

---

⭐ If you find this project useful for learning, feel free to explore the code and build upon it.
