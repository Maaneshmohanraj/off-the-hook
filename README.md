# 🦈 Off-The-Hook Mail  
**AI-Powered Phishing Detection & Cybersecurity Education Suite**

![Demo](documentation/gif.gif)

An all-in-one platform combining **AI phishing detection**, **browser integration**, and **interactive cybersecurity learning**.

---

## 🚀 Overview  
**Off-The-Hook Mail** merges a **Chrome extension**, **AI backend**, and **React-based learning tools** to detect phishing emails in real-time while teaching users how to spot them.

---

## 🧠 Core Components  
| Component | Description |
|------------|--------------|
| **Chrome Extension** | Scans Gmail emails in real time and displays AI-driven confidence scores. |
| **Model with Python Server** | Hybrid **DistilBERT + engineered features** model for phishing detection. |
| **React Game** | Gamified phishing identification trainer. |
| **Quiz Platform** | ASU-themed structured learning with real-world email scenarios. |

---

## ⚙️ Quick Setup  
**Requirements:** Python 3.8+, Node.js, npm  

### 1️⃣ Start AI Backend  
```bash
cd python-server
pip install Flask flask-cors torch transformers pandas numpy scikit-learn
python server.py
````

Model file: [Download best_model.pth](https://drive.google.com/file/d/16f8wCBMSGe6uNLx_EQmDSm206z-80EPr/view?usp=sharing)

Server runs at: [http://127.0.0.1:5000](http://127.0.0.1:5000)

---

### 2️⃣ Launch Game

```bash
cd game
npm install
npm run dev
```

Game runs at: [http://localhost:5173](http://localhost:5173)

---

### 3️⃣ Launch Quiz

```bash
cd quiz
npm install
npm start
```

Quiz runs at: [http://localhost:3000](http://localhost:3000)

---

### 4️⃣ Load Chrome Extension

1. Open Chrome → go to `chrome://extensions`
2. Enable **Developer Mode**
3. Click **Load unpacked**
4. Select the `/chrome-extension` folder

---

## 🧩 Features

* 📨 **Real-Time Email Analysis** — AI banners in Gmail detect phishing instantly.
* 📊 **Confidence Scoring** — Detailed breakdowns explaining each detection.
* 🎮 **Gamified Training** — Interactive learning through a phishing detection game.
* 🏫 **ASU-Branded Quiz** — University-style education with progress tracking.
* 📈 **Statistics Dashboard** — Monitors total scans, phishing detections, and accuracy.

---

## 🧬 AI Model

* **Architecture:** DistilBERT + 19 engineered email features
* **Training Data:** Real phishing datasets
* **Performance:** High accuracy, optimized for real-time inference
* **Notebook:** `python-server/mail.ipynb`
* **Model File:** [best_model.pth](https://drive.google.com/file/d/16f8wCBMSGe6uNLx_EQmDSm206z-80EPr/view?usp=sharing)

---

## 🧰 Troubleshooting

* Ensure **Flask**, **Game**, and **Quiz** servers are all running
* Default ports:

  * Flask API → 5000
  * Game → 5173
  * Quiz → 3000
* Reload Chrome extension after updates
* If CORS errors occur, ensure `flask-cors` is installed and configured

---

## 🧱 Repository Structure

```
/off-the-hook-mail
|-- /chrome-extension       <-- LOAD THIS IN CHROME
|   |-- manifest.json
|   |-- background.js
|   |-- content.js
|   |-- popup.html / popup.js
|   |-- /images
|
|-- /python-server          <-- AI BACKEND
|   |-- server.py
|   |-- mail.ipynb
|   |-- best_model.pth
|
|-- /game                   <-- EDUCATIONAL GAME
|   |-- package.json
|   |-- /src
|   |-- /public
|
|-- /quiz                   <-- ASU TRAINING PLATFORM
|   |-- package.json
|   |-- /src
|   |-- /public
```

---

## 🎥 Live Demo

▶️ [YouTube Video](https://youtu.be/1NUrwOtQyuA)

