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
🧠 Step 1 — Download your ZIP (if not already)

On GitHub, click on Smart-Construction-Monitoring-full.zip.

Click Download.

Extract it on your computer (e.g., Desktop or Documents folder).

⚙️ Step 2 — Open the project folder

After extracting, you’ll see:

AI_Model/
IoT_Code/
Dashboard/
docs/
requirements.txt
setup_instructions.txt

💻 Step 3 — Run the Dashboard

Open VS Code or Command Prompt / Terminal.

Navigate to the Dashboard folder:

cd Dashboard


Create a virtual environment and install dependencies:

Code:
python -m venv venv
venv\Scripts\activate  # (Windows)
pip install flask requests paho-mqtt


Run the Flask app:
python app.py


Open your browser and go to 👉 http://localhost:5000

You’ll see your dashboard running ✅

🌡️ Step 4 — Simulate IoT Sensors

Open a new terminal.

Code:
cd IoT_Code
python -m venv venv_iot
venv_iot\Scripts\activate
pip install paho-mqtt requests
python publish_test.py


You’ll see “Published …” messages.
Go back to the dashboard tab — you’ll see sensor data appear.

🧠 Step 5 — Run the AI Detection (optional)

Open another terminal.

Code:
cd AI_Model
python -m venv venv_ai
venv_ai\Scripts\activate
pip install -r requirements-ai.txt
python detect.py


It will open a webcam window or use demo.mp4 if present.
Detected objects will be sent to the dashboard.

✅ Step 6 — Done!

Now your AI + IoT + Dashboard system is running live.
All alerts and detections update every few seconds in your browser.

## 🧠 Future Scope
- Integration with BIM & GIS data  
- Drone-based visual monitoring  
- Predictive risk analysis with AI  

---

## 📜 License
This project is licensed under the **MIT License** – see the [LICENSE](LICENSE) file for details.

---

**© 2025 Naga Varshith | Smart Construction Monitoring Hackathon Project**
