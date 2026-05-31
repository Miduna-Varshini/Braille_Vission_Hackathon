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
