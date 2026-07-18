# AI-Powered Grievance Management System

An intelligent web-based grievance management platform that leverages Machine Learning to automatically classify complaints, route them to the appropriate department, and streamline grievance handling through automated email notifications.

---

## Overview

The **AI-Powered Grievance Management System** is a full-stack web application designed to simplify and automate the grievance redress process. The system enables users to register, submit complaints, and track their status while automatically classifying grievances into the appropriate department using a trained Machine Learning model.

By integrating AI-based text classification, MongoDB for data management, and SMTP email automation, the platform minimizes manual intervention and improves the efficiency of complaint handling.

---

## Features

- User Registration and Secure Authentication
- AI-Based Complaint Classification
- Automatic Department Routing
- SMTP Email Notifications
- Complaint Status Tracking
- User Dashboard
- Admin Dashboard
- Complaint Management
- Responsive User Interface
- MongoDB Integration

---

## System Workflow

```text
User Registration/Login
          │
          ▼
 Submit Complaint
          │
          ▼
 TF-IDF Vectorization
          │
          ▼
 Machine Learning Classifier
          │
          ▼
 Predict Department
          │
          ▼
 Store Complaint in MongoDB
          │
          ▼
 Send Email Notification
          │
          ▼
 Complaint Tracking Dashboard
```

---

## System Architecture

```text
User
 │
 ▼
Flask Web Application
 │
 ├── Authentication
 ├── Complaint Module
 ├── Dashboard
 │
 ▼
Machine Learning Pipeline
 │
 ├── TF-IDF Vectorizer
 ├── Complaint Classifier
 └── Label Encoder
 │
 ▼
MongoDB Database
 │
 ▼
SMTP Email Service
 │
 ▼
Concerned Department
```

---

## Machine Learning Pipeline

The complaint classification pipeline consists of:

- Text Preprocessing
- TF-IDF Vectorization
- Complaint Classification
- Label Encoding
- Department Prediction

The trained model classifies complaints into departments such as:

- Roads
- Water Supply
- Electricity
- Health
- Sanitation
- Transport
- Public Services

---

## Technology Stack

### Backend

- Python
- Flask
- Flask-PyMongo

### Database

- MongoDB

### Machine Learning

- Scikit-learn
- TF-IDF Vectorizer
- Joblib

### Frontend

- HTML5
- CSS3
- Bootstrap
- Jinja2 Templates

### Email Service

- SMTP (Gmail)

---

## Project Structure

```text
Grievance_app/
│
├── app.py
├── model/
│   ├── complaint_classifier.pkl
│   ├── tfidf_vectorizer.pkl
│   └── label_encoder.pkl
│
├── static/
│   └── style.css
│
├── templates/
│   ├── layout.html
│   ├── index.html
│   ├── login.html
│   ├── register.html
│   ├── complaint.html
│   ├── dashboard.html
│   └── admin.html
│
├── requirements.txt
└── README.md
```

---

## Installation

### Clone the repository

```bash
git clone https://github.com/GowthamRavuri01/ai-grievance-management-system.git
```

### Navigate to the project directory

```bash
cd ai-grievance-management-system
```

### Install dependencies

```bash
pip install -r requirements.txt
```

### Configure

Update the following inside `app.py`:

- MongoDB Connection URI
- Gmail SMTP Credentials

### Run the application

```bash
python app.py
```

The application will be available at:

```
http://127.0.0.1:5000
```

---

## Future Enhancements

- JWT Authentication
- Role-Based Access Control
- Complaint Priority Prediction
- Multi-language Complaint Support
- AI Chatbot Integration
- REST API Support
- Docker Deployment
- Cloud Deployment
- Analytics Dashboard

---

## Author

**Gowtham Ravuri**

AI Engineer | Computer Vision Engineer | Software Engineer

- GitHub: https://github.com/GowthamRavuri01
- LinkedIn: https://www.linkedin.com/in/gowthamravuri

---

## License

This project is licensed under the **MIT License**.
