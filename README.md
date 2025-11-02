# 🏗️ AI-Powered Smart Construction Site Monitoring System

## 🚨 Overview
An intelligent system that integrates **AI (Computer Vision)** and **IoT sensors** to monitor construction sites in real-time.  
It detects worker safety gear (helmet, vest), identifies unsafe activities, and analyzes environmental conditions to ensure safer and more efficient construction operations.

---

## 🎯 Problem Statement
Construction sites face frequent safety violations and inefficient manual monitoring.  
Traditional supervision methods are slow, error-prone, and reactive, often leading to accidents, rework, and delays.

---

## 💡 Proposed Solution
Our system automates site supervision through:
- **AI-based video analytics (YOLOv8, OpenCV)** to detect PPE compliance and unsafe activities.
- **IoT sensors** (DHT11, Gas, Motion) for real-time monitoring of site environment.
- **Cloud dashboard** (Flask + Streamlit/Firebase) for alerts, analytics, and automated reports.

---

## ⚙️ Technology Stack
| Layer | Technologies |
|--------|---------------|
| AI / CV | Python, YOLOv8, OpenCV |
| IoT | Raspberry Pi / NodeMCU, DHT11, Gas Sensor |
| Backend | Flask / FastAPI |
| Frontend | Streamlit / React + Firebase |
| Database | Firebase / MongoDB |
| Hosting | AWS / Google Cloud |

---

## 🌍 Impact
- Reduces safety risks and accidents  
- Improves project visibility and accountability  
- Enables real-time decision-making  
- Scalable to multiple sites and geographies  

---

## 🧩 Repository Structure
```
AI_Model/       → AI detection code & models
IoT_Code/       → Arduino/Python sensor scripts
Dashboard/      → Web dashboard for visualization
docs/           → Presentations and system architecture
```

---

## 💻 How to Run
### 🧠 Step 1 — Download the Project
1. On GitHub, click on **Smart-Construction-Monitoring-full.zip**.
2. Click **Download ZIP** and extract it on your computer.

You will see the following structure:
```
AI_Model/
IoT_Code/
Dashboard/
docs/
requirements.txt
setup_instructions.txt
```

---

### ⚙️ Step 2 — Run the Dashboard
1. Open **VS Code** or **Command Prompt / Terminal**.
2. Navigate to the Dashboard folder:
   ```bash
   cd Dashboard
   ```
3. Create a virtual environment and install dependencies:
   ```bash
   python -m venv venv
   venv\Scripts\activate     # (Windows)
   pip install flask requests paho-mqtt
   ```
4. Run the Flask app:
   ```bash
   python app.py
   ```
5. Open your browser and go to 👉 **http://localhost:5000**
   You’ll see your dashboard running ✅

---

### 🌡️ Step 3 — Simulate IoT Sensors
1. Open a **new terminal**.
   ```bash
   cd IoT_Code
   python -m venv venv_iot
   venv_iot\Scripts\activate
   pip install paho-mqtt requests
   python publish_test.py
   ```
   You’ll see “Published …” messages.
   Go back to the dashboard — sensor data will appear.

---

### 🧠 Step 4 — Run the AI Detection (optional)
1. Open another terminal.
   ```bash
   cd AI_Model
   python -m venv venv_ai
   venv_ai\Scripts\activate
   pip install -r requirements-ai.txt
   python detect.py
   ```
   This opens a webcam or uses `demo.mp4` to detect objects.
   Detected objects will be sent to the dashboard.

---

### ✅ Step 5 — Done!
Your **AI + IoT + Dashboard** system is now running live.
All detections and alerts update in real time!


## 🧠 Future Scope
- Integration with BIM & GIS data  
- Drone-based visual monitoring  
- Predictive risk analysis with AI  

---

## 📜 License
This project is licensed under the **MIT License** – see the [LICENSE](LICENSE) file for details.

---

**© 2025 Naga Varshith | Smart Construction Monitoring Hackathon Project**
