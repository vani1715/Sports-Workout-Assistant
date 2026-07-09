# FORMScope – AI-Based Workout Form Correction System

![Python](https://img.shields.io/badge/Python-3.11-blue?logo=python)
![MediaPipe](https://img.shields.io/badge/MediaPipe-Pose-orange)
![OpenCV](https://img.shields.io/badge/OpenCV-Computer%20Vision-green?logo=opencv)
![Flask](https://img.shields.io/badge/Flask-Web%20Dashboard-black?logo=flask)
![Status](https://img.shields.io/badge/Status-Completed-success)

---

# 📌 Overview

FORMScope is an AI-powered workout form correction system that performs **real-time human pose estimation** using a webcam and provides intelligent feedback to help users improve exercise technique.

The system combines **Google MediaPipe Pose**, **OpenCV**, **Flask**, **Computer Vision**, and **Machine Learning** to analyze body posture, calculate biomechanical joint angles, count repetitions, evaluate exercise quality, and provide instant visual, audio, and dashboard-based feedback.

Unlike traditional fitness trackers that only count repetitions, FORMScope focuses on **movement quality**, helping users perform exercises safely and efficiently.

---

# 🎯 Motivation

Incorrect exercise posture is one of the leading causes of gym-related injuries and ineffective workouts.

FORMScope aims to make professional-quality exercise guidance accessible to everyone by providing:

- 🏋️ Real-time workout posture correction
- 🎯 Biomechanical form analysis
- 🔊 Instant voice feedback
- 📊 Live exercise scoring
- 💻 Browser-based monitoring dashboard
- 🏠 Completely offline processing

The project demonstrates how **Artificial Intelligence**, **Computer Vision**, and **Sports Biomechanics** can be combined to build an intelligent virtual fitness assistant.

---

# 📂 Project Structure

```
FORMScope/
│
├── exercises/
│   ├── base.py
│   ├── exercises.py
│
├── utils/
│   ├── angles.py
│   ├── tts.py
│   └── helpers.py
│
├── server/
│   ├── app.py
│   ├── templates/
│   └── static/
│
├── models/
│   └── knn_model.pkl
│
├── assets/
│
├── main.py
├── requirements.txt
├── README.md
└── .gitignore
```

---

# 🧠 Key Modules

### 📷 Pose Detection

- Captures live webcam feed
- Detects 33 body landmarks using MediaPipe Pose
- Tracks body movement in real time
- Generates landmark coordinates for further analysis

---

### 📐 Joint Angle Computation

- Calculates elbow angles
- Computes knee angles
- Hip angle estimation
- Spine alignment analysis
- Body posture assessment
- Smooths angle values for stable predictions

---

### 🏋️ Exercise Analysis

Implements dedicated biomechanical models for:

- Squats
- Push-Ups
- Planks
- Lunges
- Bicep Curls

Each exercise contains:

- Form validation
- Repetition counting
- Joint-specific scoring
- Personalized feedback

---

### 🤖 Machine Learning Module

Uses a **K-Nearest Neighbour (KNN)** classifier to detect improper torso leaning during **Bicep Curl** exercises.

The model:

- Extracts pose-based features
- Normalizes landmark coordinates
- Classifies correct and incorrect posture
- Achieves over **94% classification accuracy**

---

### 🌐 Dashboard

Provides a real-time web interface built using Flask.

Features include:

- Live video stream
- Current exercise
- Form score
- Repetition count
- Feedback messages
- Session controls
- Exercise switching

---

### 🔊 Voice Feedback

Uses **pyttsx3** to generate offline speech.

The voice engine runs on a dedicated thread, allowing:

- Non-blocking execution
- Continuous real-time feedback
- Smooth video processing

---

# 🏋️ Supported Exercises

- ✅ Squat
- ✅ Push-Up
- ✅ Plank
- ✅ Lunge
- ✅ Bicep Curl

---

# ⚙️ Technologies Used

### Programming Language

- Python

### Computer Vision

- OpenCV
- MediaPipe Pose

### Machine Learning

- Scikit-learn
- K-Nearest Neighbour (KNN)

### Backend

- Flask
- Flask-Sock (WebSocket)

### Audio

- pyttsx3

### Scientific Computing

- NumPy

---

# 🚀 Features

- Real-time pose estimation
- Joint angle calculation
- Exercise repetition counting
- Biomechanical posture analysis
- AI-based form correction
- Voice-assisted coaching
- Live web dashboard
- Offline processing
- CPU-only execution
- Extensible modular architecture

---

# 📈 Performance

- **33 body landmarks tracked**
- **Real-time processing (~30 FPS)**
- **~11.5 ms average processing latency**
- **CPU-only execution**
- **94.3% KNN posture classification accuracy**
- **Offline operation (No cloud dependency)**

---

# 🔮 Future Improvements

- Mobile application
- User authentication
- Workout history tracking
- Progress analytics
- Cloud synchronization
- Additional exercise support
- Deep Learning posture classification
- Personalized workout recommendations
- Multi-camera pose estimation
- 3D body pose analysis

---

# ⚖️ Disclaimer & Ownership

This project is an original academic work developed by Shreyas Sahoo along with contributing team members as part of coursework and learning in Sports & Athletics.

This project is intended strictly for educational and academic use. Unauthorized commercial use, redistribution without proper credit, or plagiarism of this work—either in full or in part—is not permitted. The authors assume no responsibility for any misuse of this project or its outcomes. If this project is referenced, reused, or built upon, clear and proper attribution to the authors and team members is mandatory. 
