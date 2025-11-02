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

## 🎥 Demo Video
*(Add your YouTube/Drive demo link here)*

---

## 💻 How to Run
1. Clone the repository:
   ```bash
   git clone https://github.com/yourusername/Smart-Construction-Monitoring.git
   cd Smart-Construction-Monitoring
   ```
2. Install dependencies:
   ```bash
   pip install -r requirements.txt
   ```
3. Run the dashboard:
   ```bash
   python Dashboard/app.py
   ```
4. Open your browser and go to `http://localhost:5000`

---

## 🧠 Future Scope
- Integration with BIM & GIS data  
- Drone-based visual monitoring  
- Predictive risk analysis with AI  

---

## 📜 License
This project is licensed under the **MIT License** – see the [LICENSE](LICENSE) file for details.

---

**© 2025 Naga Varshith | Smart Construction Monitoring Hackathon Project**
