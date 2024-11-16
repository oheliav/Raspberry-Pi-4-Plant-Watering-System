# Raspberry Pi 4 Plant Watering System

## 🌱 Project Overview
This project automates plant watering using a **Raspberry Pi 4**, soil moisture sensors, and a water pump. It's perfect for keeping your plants healthy while you're away! 🌿

### Features
- Automatically waters plants when soil moisture levels are low.
- Monitors soil moisture levels in real-time.
- Provides a web-based interface to monitor and control the system.
- Logs data for tracking soil and watering trends.
- Optional: Integrate a camera for live plant monitoring.

---

## 🚀 Getting Started

### Hardware Requirements
- **Raspberry Pi 4** (any model with GPIO pins)
- **Soil moisture sensor**
- **Relay module**
- **Water pump** or **solenoid valve**
- Tubing for water delivery
- Breadboard and jumper wires
- Optional: DHT11/DHT22 for temperature and humidity
- Optional: Camera module

---

## 🛠️ Software Requirements
- Python 3
- Flask (for the web interface)
- Raspberry Pi GPIO library
- SQLite (optional, for data logging)

---

## 🔧 Installation & Setup
1. **Clone the Repository**:
   git clone https://github.com/oheliav/raspi-plant-watering.git

2. Install Dependencies:
   pip install flask RPi.GPIO

3. Connect the Hardware:
  - Connect the soil moisture sensor to the Raspberry Pi GPIO pins.
  - Wire the relay to control the water pump.
  - Set up the water pump with the tubing.

4. Run the Application:
   python src/main.py

5. Access the Dashboard:
  Open your browser and go to http://<raspi-ip>:5000

📂 Project Structure
raspi-plant-watering/
│
├── src/
│   ├── sensors.py         # Sensor interaction code
│   ├── pump_control.py    # Water pump control logic
│   ├── app.py             # Flask web application
│   └── main.py            # Main script
│
├── docs/
│   ├── wiring_diagram.png # Hardware setup diagram
│   └── flowchart.png      # Project workflow
│
├── logs/
│   └── watering.log       # Logs moisture levels and watering events
│
└── README.md              # Project documentation

🖼️ Preview

🔮 Future Improvements
  - Add temperature and humidity monitoring.
  - Implement scheduled watering.
  - Build a mobile app interface.
  - Include AI-based recommendations for plant care.

🤝 Contributing
Feel free to fork this repository and contribute! Submit a pull request with your improvements.

📜 License
This project is licensed under the MIT License.
