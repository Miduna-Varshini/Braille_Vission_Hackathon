*# ⠃ BrailleVision — Physical Braille to English using Camera AI

> Real-time physical Braille recognition using CNN + OpenCV + Streamlit

[![Streamlit App](https://img.shields.io/badge/Streamlit-Live%20App-FF4B4B?logo=streamlit)](https://braille-hackathon-rgiodfqrpcjssu6yku77wf.streamlit.app/)
[![Python](https://img.shields.io/badge/Python-3.11-blue?logo=python)](https://python.org)
[![TensorFlow](https://img.shields.io/badge/TensorFlow-2.x-orange?logo=tensorflow)](https://tensorflow.org)

---

## 🎯 Problem Statement

Braille is the primary reading system for visually impaired people worldwide.
But most people around them — teachers, family members, and caregivers —
cannot read Braille. BrailleVision solves this by instantly converting
physical Braille into spoken English using just a camera.

---

## ✅ What BrailleVision Does

- 📷 Accepts real Braille images via upload or live camera
- 🔬 Uses OpenCV to detect and segment Braille dot cells
- 🧠 CNN model predicts each letter with 99% accuracy
- 🔊 Reads the recognized text aloud using Text to Speech
- 🌐 Deployed as a web app — works on any device

---

## 🛠️ Tech Stack

| Tool | Purpose |
|---|---|
| Python | Programming language |
| TensorFlow / Keras | CNN model training |
| OpenCV | Image processing & dot detection |
| ONNX Runtime | Fast model inference on Streamlit Cloud |
| Streamlit | Web app interface |
| gTTS | Text to speech output |
| Google Colab | Model training with T4 GPU |

---

## 🧠 Model Architecture**
Input (50x50 grayscale)
↓
Conv2D (32 filters) → MaxPooling
↓
Conv2D (64 filters) → MaxPooling
↓
Conv2D (128 filters) → MaxPooling
↓
Flatten → Dense (256) → Dropout (0.5)
↓
Dense (26) → Softmax
↓
Output: A to Z

### Training Results
- Dataset: 2080 images, 26 classes (A–Z)
- Epochs: 20
- Optimizer: Adam
- Training Accuracy: **99%**
- Validation Accuracy: **100%**

---

## 🔍 How It Works

**Step 1 — Capture**
User uploads a Braille image or scans using live camera.

**Step 2 — Detect**
OpenCV converts image to grayscale, applies thresholding,
detects Braille dot columns and segments each character cell.

**Step 3 — Predict**
Each cell is fed to the CNN model which predicts the letter.
All letters are joined to form the complete text.

**Step 4 — Speak**
gTTS converts the recognized text to speech and plays it aloud.

---

## 🚀 Run Locally

```bash
# Clone the repo
git clone https://github.com/codelovecore23/Braille-Hackathon.git
cd Braille-Hackathon

# Install dependencies
pip install -r requirements.txt

# Run the app
streamlit run app.py
```

---

## 📦 Requirements
