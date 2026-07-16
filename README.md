# 🚨 Real-Time AI-Powered Fraud Detection System

[![Python](https://img.shields.io/badge/Python-3.11-blue.svg)](https://www.python.org/)
[![FastAPI](https://img.shields.io/badge/FastAPI-Backend-green.svg)](https://fastapi.tiangolo.com/)
[![Streamlit](https://img.shields.io/badge/Streamlit-Dashboard-red.svg)](https://streamlit.io/)
[![Scikit-Learn](https://img.shields.io/badge/Scikit--Learn-ML-orange.svg)](https://scikit-learn.org/)
[![XGBoost](https://img.shields.io/badge/XGBoost-Classifier-blue.svg)](https://xgboost.ai/)

## 📌 Project Overview

The **Real-Time AI-Powered Fraud Detection System** is an end-to-end Machine Learning application designed to detect fraudulent financial transactions in real time. The project combines data preprocessing, feature engineering, machine learning, API deployment, and an interactive dashboard to simulate a production-grade fraud detection pipeline used in fintech organizations.

The application predicts the probability of fraud and classifies each transaction into one of three business decisions:

- ✅ **ALLOW**
- ⚠️ **REVIEW**
- 🚫 **BLOCK**

---

# 🏗️ System Architecture

```
                Financial Transaction
                        │
                        ▼
              Feature Engineering Pipeline
                        │
                        ▼
              Machine Learning Model
              (XGBoost / Isolation Forest)
                        │
                        ▼
                  FastAPI Backend
                        │
        ┌───────────────┴───────────────┐
        ▼                               ▼
 Streamlit Dashboard            REST API Clients
        │
        ▼
 Risk Score + Fraud Decision
        │
        ▼
 Logging • Monitoring • Alerts
```

---

# 🎯 Business Problem

Financial institutions process millions of transactions every day, making manual fraud detection inefficient and costly.

This project automates fraud detection by:

- Predicting fraudulent transactions in real time
- Reducing manual investigation effort
- Prioritizing high-risk transactions
- Supporting risk-based business decisions

---

# 📊 Dataset

**Dataset:** PaySim Mobile Money Fraud Detection Dataset

**Source:** Kaggle

https://www.kaggle.com/datasets/ealaxi/paysim1

### Dataset Statistics

| Attribute | Value |
|------------|--------|
| Records | 6,362,620 |
| Features | 11 |
| Target | isFraud |
| Domain | FinTech |

---

# ⚙️ Tech Stack

## Programming

- Python

## Machine Learning

- Scikit-learn
- XGBoost
- Isolation Forest

## Data Processing

- Pandas
- NumPy

## Backend

- FastAPI
- Uvicorn
- Pydantic

## Frontend

- Streamlit

## Deployment

- Local Deployment
- REST API

## MLOps

- Logging
- Model Monitoring
- Risk Scoring Engine

## Version Control

- Git
- GitHub

---

# 📂 Project Structure

```
fraud-detection/
│
├── api/
│   └── app.py
│
├── dashboard/
│   └── app.py
│
├── models/
│   └── fraud_model.pkl
│
├── notebooks/
│   └── fraud_detection.ipynb
│
├── requirements.txt
│
├── README.md
│
└── .gitignore
```

---

# 🔄 Project Workflow

### Step 1

Data Collection

↓

### Step 2

Data Cleaning & Feature Engineering

↓

### Step 3

Model Training

↓

### Step 4

Model Evaluation

↓

### Step 5

Risk Scoring

↓

### Step 6

FastAPI Deployment

↓

### Step 7

Streamlit Dashboard

↓

### Step 8

Monitoring & Logging

---

# 📈 Machine Learning Pipeline

- Data Cleaning
- Feature Engineering
- One-Hot Encoding
- Train-Test Split
- Class Imbalance Handling
- Model Training
- Hyperparameter Tuning
- Model Evaluation
- Model Serialization
- Real-Time Prediction

---

# 📊 Model Evaluation

**Final Model:** XGBoost Classifier

| Metric | Score |
|---------|--------|
| Accuracy | XX.XX% |
| Precision | XX.XX% |
| Recall | XX.XX% |
| F1 Score | XX.XX% |
| ROC-AUC | XX.XX |

> Replace the values above with your final evaluation metrics.

---

# 🚀 Features

✅ End-to-End ML Pipeline

✅ Real-Time Fraud Prediction

✅ REST API using FastAPI

✅ Interactive Streamlit Dashboard

✅ Risk Decision Engine

✅ Logging & Monitoring

✅ Modular Project Structure

✅ Production-Ready Design

---

# 🔍 API Endpoint

### POST `/predict`

Example Request

```json
{
    "amount":100000,
    "oldbalanceOrg":50000,
    "newbalanceOrig":40000,
    "oldbalanceDest":0,
    "newbalanceDest":10000,
    "type_TRANSFER":1,
    "type_CASH_OUT":0
}
```

Example Response

```json
{
    "fraud_probability":0.8149,
    "decision":"REVIEW"
}
```

---

# 🖥️ Dashboard

The Streamlit dashboard provides:

- Real-time transaction prediction
- Fraud probability visualization
- Risk decision display
- Interactive user inputs

---

#  Installation

Clone the repository

```bash
git clone https://github.com/yourusername/fraud-detection-system.git
```

Install dependencies

```bash
pip install -r requirements.txt
```

Run FastAPI

```bash
cd api
uvicorn app:app --reload
```

Run Streamlit

```bash
cd dashboard
streamlit run app.py
```

---

#  Future Enhancements

- Docker Containerization
- AWS / Azure Deployment
- Kafka-based Real-Time Streaming
- MLflow Experiment Tracking
- Prometheus & Grafana Monitoring
- Automated Model Retraining
- CI/CD Pipeline using GitHub Actions

---

#  Skills Demonstrated

- Machine Learning
- Fraud Detection
- Risk Analytics
- FastAPI
- Streamlit
- REST API Development
- Feature Engineering
- Model Deployment
- Python
- Git & GitHub
- MLOps Fundamentals

---

#  Business Impact

- Enables real-time fraud detection
- Reduces financial losses
- Improves operational efficiency
- Supports fraud analysts with automated risk scoring
- Demonstrates production-style ML deployment

---

#  Author

**Sonali Nidhi**

- LinkedIn: https://www.linkedin.com/in/sonali-nidhi-315973239/
- GitHub: https://github.com/SonaliNidhi

---

## ⭐ If you found this project interesting, consider giving it a Star!
