# 🤖 AI Mask Compliance Monitor

A real-time **AI-powered face mask detection system** built with **TensorFlow.js** and **BlazeFace**, running entirely in the browser — no server required!  
It detects faces via webcam feed and classifies whether a person is **wearing a mask** or **not**, with live dashboard stats, alerts, and sounds.

🌐 **Live Demo:** [AI Mask Compliance Monitor](https://lovnishverma.github.io/AI-Mask-Compliance-Monitor/)

---

## 🧠 Model Training (Google Colab)

You can retrain or fine-tune your own mask detection model using the following Colab notebook:  
👉 [Train Mask Detection Model on Google Colab](https://colab.research.google.com/drive/17DD8CiwwxjR_NTrCB4Ot8ymjW9NrTrNl#scrollTo=ljIrS_RG5zp4)

The notebook trains a custom CNN model, exports it to TensorFlow.js format, and provides `model.json` and `.bin` files used in this web app.

---

## ✨ Features

- 🎥 Real-time face detection using **BlazeFace**
- 😷 Mask/No-Mask classification using **TensorFlow.js**
- ⚡ Fully on-device inference (no backend or API calls)
- 🔔 Audio and visual alerts for “No Mask” detections
- 📊 Live statistics dashboard:
  - Current mask & no-mask count  
  - Total detections  
  - Real-time FPS counter
- ⚠️ Animated red banner when violation detected
- 🧩 Lightweight & runs in any modern browser

---

## 🛠️ Tech Stack

| Component | Technology Used |
|------------|------------------|
| **Frontend** | HTML5, CSS3, JavaScript (ES6) |
| **AI Models** | TensorFlow.js, BlazeFace |
| **Visualization** | Canvas 2D API |
| **Training** | TensorFlow / Keras (Colab) |
| **Deployment** | GitHub Pages |

---

## 🚀 Getting Started

### 1️⃣ Clone the repository
```bash
git clone https://github.com/Lovnishverma/AI-Mask-Compliance-Monitor.git
cd AI-Mask-Compliance-Monitor
````

### 2️⃣ Project Structure

```
AI-Mask-Compliance-Monitor/
│
├── index.html                # Main web app
├── model_web/
│   ├── model.json
│   └── group1-shard1of1.bin  # Trained model weights
├── README.md
└── assets/                   # (optional) screenshots, icons, etc.
```

### 3️⃣ Run Locally

You can simply open the `index.html` file in your browser, or use a local web server:

```bash
# Using VSCode Live Server or Python
python -m http.server 8080
```

Then open:

```
http://localhost:8080
```

> 🔐 Note: For webcam access, browsers require HTTPS or localhost.

---

## 🧩 Model Folder Setup

Make sure your `model_web` folder contains the exported TensorFlow.js files:

```
model_web/
├── model.json
└── group1-shard1of1.bin
```

If you trained your own model in Colab, download the exported files and place them in this folder.

---

## 🎯 How It Works

1. Uses **BlazeFace** to detect faces from webcam frames.
2. Crops the face region and feeds it into the mask classification model.
3. Predicts whether the person is **wearing a mask** or **not wearing a mask**.
4. Displays real-time bounding boxes, confidence levels, and dashboard stats.
5. Plays an audio alert + flashes red banner for violations.

---

## 📸 Screenshot (Preview)

<img width="1918" height="1007" alt="image" src="https://github.com/user-attachments/assets/062cd7cf-2b34-4c5f-8680-f2fa94392659" />


<img width="1918" height="1078" alt="image" src="https://github.com/user-attachments/assets/a8d377c9-fcb4-4ca7-9fcd-34828ae8aff8" />


---

## 📡 Deployment

This project is live on **GitHub Pages**:
➡️ **[https://lovnishverma.github.io/AI-Mask-Compliance-Monitor/](https://lovnishverma.github.io/AI-Mask-Compliance-Monitor/)**

To redeploy after edits:

```bash
git add .
git commit -m "Update project"
git push origin main
```

---

## 💡 Future Enhancements

* Add **live chart** for mask compliance trends
* Store detection logs using **Firebase / IndexedDB**
* Multi-person tracking with unique IDs
* Improved alert system with voice feedback

---

## 👨‍💻 Author

**Lovnish Verma**
🔗 [GitHub](https://github.com/Lovnishverma)
🎓 [ResearchGate](https://www.researchgate.net/profile/Lovnish-Verma)
📺 [YouTube Channel](https://www.youtube.com/@lovnishverma)
✍️ [Medium Blog](https://lovnish.medium.com/)

---

## 📝 License

This project is licensed under the **MIT License** — free to use and modify with attribution.

---

**Made with ❤️ using TensorFlow.js, BlazeFace, and OpenCV-inspired techniques.**

