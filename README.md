# 🎤 Audio Based Emotion Detection System

## 📌 Introduction

Human emotions play a vital role in communication. Understanding emotional cues from speech can significantly enhance human-computer interaction, mental health monitoring, customer service analytics, and many other domains. This project presents an **Audio Based Emotion Detection System** that classifies human emotions (e.g., happy, sad, angry, neutral, fearful, surprised, disgusted) from speech signals.

The system leverages a hybrid **CNN (Convolutional Neural Network) + LSTM (Long Short-Term Memory)** architecture to capture both spatial (spectral) and temporal features from audio. A Flask backend serves the trained model, while a responsive frontend built with HTML, CSS, and JavaScript allows users to upload or record audio and receive real-time emotion predictions.

---

## 🧠 What is this project about?

This project is an end-to-end machine learning web application that:

- **Accepts audio input** (WAV format) from a user via file upload or microphone recording.
- **Preprocesses** the audio by extracting **Mel-frequency cepstral coefficients (MFCCs)** – a compact representation of the audio spectrum that mimics human auditory perception.
- **Feeds** the processed features into a pre-trained **CNN-LSTM model**.
  - **CNN layers** learn local patterns and high-level feature maps from MFCC spectrograms.
  - **LSTM layers** capture long-term dependencies and sequential relationships across time frames.
- **Outputs** the predicted emotion label with confidence scores.
- **Visualizes** the result on a clean, interactive web dashboard.

The system bridges the gap between deep learning research and practical deployment, demonstrating how speech emotion recognition (SER) can be made accessible through a browser interface – even with moderate accuracy, providing a baseline for further improvements.

---

## ✨ Features

- 🎙️ Upload audio file (`.wav`) or record live audio from microphone
- 🧹 Automatic noise reduction and silence trimming
- 📊 Real-time emotion prediction with probability bars
- 📈 Visual waveform preview of uploaded/recorded audio
- 🖥️ Responsive UI (mobile & desktop friendly)
- ⚡ Fast inference using Flask + pre-trained model
- 🔁 REST API endpoint for programmatic access

---

## 🛠️ Tech Stack

| Layer       | Technology                                                                 |
|-------------|----------------------------------------------------------------------------|
| **ML Model**| TensorFlow / Keras – CNN + LSTM                                            |
| **Backend** | Flask (Python)                                                             |
| **Frontend**| HTML5, CSS3, JavaScript (Vanilla) + Web Audio API / RecordRTC              |
| **Audio Processing** | Librosa (MFCC extraction), NumPy, SciPy                          |
| **Deployment** (optional) | Gunicorn, Docker, or any cloud platform (AWS, Heroku, etc.)    |

---
