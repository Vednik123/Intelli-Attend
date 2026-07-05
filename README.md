# IntelliAttend
### AI-Based Face & Voice Attendance System

<p align="center">
  <img src="https://img.shields.io/badge/Python-3.10+-blue.svg">
  <img src="https://img.shields.io/badge/Streamlit-Frontend-red.svg">
  <img src="https://img.shields.io/badge/Supabase-PostgreSQL-green.svg">
</p>

---

## 📖 Overview

**IntelliAttend** is an AI-powered attendance management system that automates classroom attendance using **Face Recognition** and **Voice Recognition**.

The system provides two user roles:

- 👨‍🏫 Teacher
- 👨‍🎓 Student

Teachers can capture classroom images to automatically mark attendance, while students can also verify their attendance using voice authentication.

The project combines Computer Vision, Machine Learning, Audio Processing, and Cloud Database technologies to provide a secure and efficient attendance solution.

---

# ✨ Features

## 👨‍🏫 Teacher Module

- Teacher Registration & Login
- Create Subjects
- Generate QR Code for Class
- Create New Classes
- Capture Classroom Image
- Automatic Face Detection
- Automatic Attendance Marking
- View Attendance Records

---

## 👨‍🎓 Student Module

- Student Registration
- Face Registration
- Voice Registration
- Join Subject using QR Code

---

## 🤖 AI Features

### Face Recognition

- Face Detection using dlib
- Facial Landmark Detection
- Face Alignment
- 128-Dimensional Face Embeddings
- Student Classification using Support Vector Classifier (SVC)

---

### Voice Recognition

- Audio Recording
- Audio Preprocessing
- Voice Embeddings
- Voice-Based Attendance Authentication

---

# 🧠 Working

## Face Attendance Workflow

```
Teacher Captures Class Image
          │
          ▼
Detect Faces
          │
          ▼
Extract Face Embeddings
          │
          ▼
Compare with Registered Students
          │
          ▼
Identify Student using SVC
          │
          ▼
Attendance Marked
```

---

## Voice Attendance Workflow

```
Student Says "Present"
          │
          ▼
Audio Recording
          │
          ▼
Audio Preprocessing
          │
          ▼
Voice Embedding Extraction
          │
          ▼
Speaker Verification
          │
          ▼
Attendance Marked
```

---

# 🏗️ Project Architecture

```
IntelliAttend
│
├── app.py
├── requirements.txt
├── src
│   ├── screens
│   │     ├── home_screen.py
│   │     ├── teacher_screen.py
│   │     └── student_screen.py
│   │
│   ├── components
│   │
│   ├── pipelines
│   │     ├── face_pipeline.py
│   │     └── voice_pipeline.py
│   │
│   ├── database
│   │     └── db.py
│   │
│   └── utils
│
├── ui
│
├── .streamlit
│     └── secrets.toml
│
└── assets
```

---

# 🛠️ Tech Stack

## Frontend

- Streamlit
- HTML
- CSS

---

## Backend

- Python

---

## Database

- Supabase
- PostgreSQL

---

## Machine Learning

- Scikit-Learn
- Support Vector Classifier (SVC)

---

## Face Recognition

- dlib
- face_recognition
- ResNet Face Embeddings

---

## Voice Recognition

- Librosa
- Resemblyzer

---

## Authentication

- Supabase Authentication
- bcrypt Password Hashing

---

## QR Code

- Segno

---

## Image Processing

- Pillow

---

# 📦 Libraries Used

```
numpy
pandas
scikit-learn
dlib
face_recognition
librosa
resemblyzer
pillow
segno
bcrypt
streamlit
supabase
```

---

# 🔒 Security

- Password Hashing using bcrypt
- Secure Authentication
- Face Embedding Storage
- Voice Embedding Storage
- Cloud Database (Supabase)

---

# ⚙️ Installation

Clone the repository

```bash
git clone https://github.com/your-username/IntelliAttend.git
```

Go to project folder

```bash
cd IntelliAttend
```

Create Virtual Environment

Windows

```bash
python -m venv venv
```

Activate

```bash
venv\Scripts\activate
```

Linux / Mac

```bash
source venv/bin/activate
```

Install Dependencies

```bash
pip install -r requirements.txt
```

Run Application

```bash
streamlit run app.py
```

---

# 🔑 Environment Variables

Create

```
.streamlit/secrets.toml
```

Example

```toml
SUPABASE_URL="YOUR_SUPABASE_URL"
SUPABASE_KEY="YOUR_SUPABASE_KEY"
```

---

# 🚀 Deployment

## Streamlit Cloud

To deploy the webpage having all the functionalities.

## Landing Page

A separate landing page is deployed using **Vercel**, which redirects users to the Streamlit application.


---

# 🎯 Project Objectives

- Eliminate Manual Attendance
- Improve Attendance Accuracy
- Prevent Proxy Attendance
- Fast Student Identification
- Secure Authentication
- Cloud-Based Data Management

---

## ⭐ If you found this project useful, don't forget to Star the repository!
