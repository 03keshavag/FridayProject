# 🤖 FRIDAY – AI-Powered Desktop Personal Assistant

FRIDAY is an advanced **AI-powered desktop personal assistant** built using Python.
It combines **voice control**, **computer vision**, **system automation**, **real-time dashboards**, and **peer-to-peer communication** into a single intelligent ecosystem.

FRIDAY runs locally on your machine and interacts through a floating **Orb UI**, voice commands, and a web-based control panel.

---

## ✨ Key Features

### 🗣️ Voice Assistant

* Speech recognition using microphone input
* Natural language responses via LLM (Groq-compatible OpenAI API)
* Text-to-Speech (TTS) voice output
* Wake-word activation (`Hey Friday`)

### 🟢 Floating Orb UI

* Always-on-top animated orb using **PyQt5**
* Visual states:

  * Idle (white)
  * Listening (green)
  * Speaking (blue)
* Smooth pulsing and floating animation

### 🖥️ System Automation

* Open & close installed applications
* Create and delete files/folders
* Control:

  * Mouse movement & clicks
  * Keyboard shortcuts
  * Volume & brightness
* Screenshot capture + OCR text reading

### 🌐 Web Dashboard

* Flask-based web interface
* Start / Stop FRIDAY from browser
* Live status monitoring
* Meme & News dashboard

### 🌱 EcoSystem Monitor

* Real-time system monitoring using Streamlit
* CPU, RAM, Disk usage
* Power consumption estimation
* Carbon footprint estimation
* Eco-score (1–10) with recommendations

### 📡 Peer-to-Peer Communication

* WebSocket-based messaging system
* Multiple FRIDAY instances (Friday1 ↔ Friday2)
* Send voice messages between systems in real time

### 🎮 Vision-Based Game Control

* Head-tilt steering for browser games
* Powered by OpenCV + MediaPipe

### 🚨 Emergency System

* Emergency SMS alerts via Twilio
* Sends real-time alerts to caretaker

---

## 🏗️ Project Architecture

```
FRIDAY/
│
├── orb.py              # Core assistant + Orb UI + voice logic
├── backend.py          # Flask backend (start/stop FRIDAY)
├── eco.py              # Streamlit EcoSystem Monitor
├── server.py           # WebSocket relay server
├── friday2.py          # Second FRIDAY client (peer assistant)
│
├── index.html          # Web control UI
├── static/
│   ├── script.js       # Frontend control logic
│   ├── styles.css      # UI styling
│
├── apps_cache.json     # Cached installed apps
└── README.md
```

---

## ⚙️ Technologies Used

* **Python**
* **Flask**
* **Streamlit**
* **PyQt5**
* **OpenCV**
* **MediaPipe**
* **SpeechRecognition**
* **pyttsx3**
* **WebSockets**
* **Twilio**
* **Groq**

---

## 🚀 How to Run

### 1️⃣ Start WebSocket Server

```bash
python server.py
```

### 2️⃣ Start Web Controller

```bash
python backend.py
```

Open browser:

```
http://localhost:5000
```

### 3️⃣ Start FRIDAY (Orb Assistant)

Use **Start FRIDAY** button from the web UI
or run directly:

```bash
python orb.py
```

### 4️⃣ Optional: Start Second Assistant

```bash
python friday2.py
```

---

## 🔐 Configuration Notes

* Replace API keys:

  * Groq / OpenAI API key
  * Twilio SID, Auth Token, Phone Numbers
* Ensure Tesseract OCR is installed and path is correct
* Microphone & camera permissions required

---

## 🎯 Use Cases

* Personal desktop automation
* Voice-controlled system assistant
* Assistive technology
* Smart system monitoring
* Hackathons & research projects
* AI + HCI experimentation

---

## 📌 Future Enhancements

* Wake-word engine (offline)
* Mobile companion app
* Encrypted P2P messaging
* Plugin-based command system
* Multi-language voice support

---


## 📜 License

This project is intended for **educational and research purposes**.
Feel free to fork, modify, and experiment responsibly.


