
# Smart Construction Monitoring System

A real-time AI + IoT-based construction site monitoring platform to ensure safety, progress tracking, and efficiency.

---

## 🚀 How to Run the Project (Step-by-Step)

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

---

### 💡 Optional: Deploy Online
You can host the dashboard using:
- **Render / Railway / Vercel (Flask deployment)**
- **AWS EC2 or Heroku (for IoT + Flask)**

---

### 📦 Tech Stack
- **Backend:** Flask (Python)
- **Frontend:** HTML, CSS, JavaScript (Chart.js)
- **IoT:** MQTT (Simulated via Paho MQTT client)
- **AI Model:** OpenCV / YOLO (optional)
- **Database:** SQLite / In-memory JSON

---

### 👨‍💻 Author
Developed by **Naga Varshith**  
For the **Smart Construction Site Monitoring Hackathon 2025**
