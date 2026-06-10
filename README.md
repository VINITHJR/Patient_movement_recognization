# AI-Based Hospital Patient Monitoring System

## Overview

The AI-Based Hospital Patient Monitoring System is an intelligent healthcare monitoring platform designed to improve patient safety through computer vision and real-time health condition detection.

The system analyzes patient video footage using MediaPipe and OpenCV to detect critical health events such as:

* Fall Detection
* Seizure Detection
* Chest Pain Detection

The platform also includes patient management functionality with PostgreSQL database integration for storing and managing patient information.

---

## Features

### Patient Management

* Add new patient records
* Store patient details securely
* View patient information
* PostgreSQL database integration

### AI Health Monitoring

* Real-time video analysis
* Fall detection using body pose estimation
* Seizure detection using motion analysis
* Chest pain detection using facial and body posture analysis

### Hospital Dashboard

* Room management interface
* Patient video monitoring
* Detection result reporting
* User-friendly web interface

---

## Technologies Used

### Frontend

* HTML
* CSS
* JavaScript

### Backend

* Python
* Flask
* Flask-CORS

### Database

* PostgreSQL
* Aiven Cloud Database

### Computer Vision & AI

* OpenCV
* MediaPipe
* NumPy

---

## System Architecture

Patient Video
↓
Health Detection Engine
↓
MediaPipe Pose & Face Mesh
↓
Condition Analysis
↓
Detection Results
↓
Hospital Dashboard

Patient Form
↓
Flask Backend
↓
PostgreSQL Database
↓
Patient Records

---

## Project Structure

```text
doctor/
│
├── app.py
├── health_detection.py
├── requirements.txt
│
├── templates/
│   ├── hospital.html
│   ├── form.html
│   └── patients.html
│
├── static/
│   ├── videos/
│   └── images/
│
└── README.md
```

---

## Installation

## Python Version

This project was developed and tested using:

```text
Python 3.12.3
```

### Recommended Version

```text
Python 3.11.x or Python 3.12.x
```

### Important

MediaPipe compatibility issues may occur with newer Python versions.

For best results, use:

```text
Python 3.12.3
```

Check your Python version:

```bash
python --version
```

### Clone Repository

```bash
git clone https://github.com/yourusername/ai-hospital-monitoring.git
cd ai-hospital-monitoring
```

### Create Virtual Environment

```bash
python -m venv .venv
```

### Activate Virtual Environment

Windows:

```bash
.venv\Scripts\activate
```

Linux / Mac:

```bash
source .venv/bin/activate
```

### Install Dependencies

```bash
pip install -r requirements.txt
```

---

## Database Configuration

Configure PostgreSQL database settings inside:

```python
app.py
```

Example:

```python
DATABASE_URL = "postgresql://username:password@host:port/database"
```

---

## Running the Project

### Start Patient Management Backend

```bash
python app.py
```

Runs on:

```text
http://127.0.0.1:5000
```

### Start Health Detection Service

```bash
python health_detection.py
```

Runs on:

```text
http://127.0.0.1:5001
```

---

## Detection Capabilities

### Fall Detection

Detects sudden downward body movement and possible falls using pose landmarks.

### Seizure Detection

Detects abnormal repetitive body motion through wrist and head movement tracking.

### Chest Pain Detection

Detects chest-holding gestures, facial discomfort, and posture changes indicating possible chest pain.

---

## Future Enhancements

* Real-time CCTV integration
* Multi-patient monitoring
* SMS and Email alerts
* AI-generated medical reports
* Nurse and doctor notification system
* Cloud deployment
* Mobile application support

---

## Applications

* Hospitals
* Elderly Care Centers
* Assisted Living Facilities
* Home Healthcare Monitoring
* Emergency Response Systems

---

## Authors

Vinith J R

Final Year Engineering Project

AI-Based Hospital Patient Monitoring System

---

## License

This project is developed for educational and research purposes.
