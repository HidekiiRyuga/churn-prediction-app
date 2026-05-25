# Customer Churn Prediction Backend

Backend API for the Customer Churn Prediction System built using FastAPI and Scikit-learn.

This backend handles:
- customer data preprocessing
- feature engineering
- machine learning inference
- churn probability prediction

---

# Live API

[backend link](https://churn-prediction-app-90ii.onrender.com/)

---

# Features

- FastAPI REST API
- Pretrained ML pipeline
- Automatic preprocessing
- Feature engineering support
- Probability-based predictions
- JSON API responses
- Production-ready deployment

---

# Machine Learning Workflow

## Models Evaluated

- Logistic Regression
- Random Forest
- Gradient Boosting
- AdaBoost
- Support Vector Classifier

Gradient Boosting achieved the best ROC-AUC performance.

---

# Final Model Performance

| Metric | Score |
|---|---|
| Accuracy | 0.8680 |
| Precision | 0.7804 |
| Recall | 0.4889 |
| F1-score | 0.6012 |
| ROC-AUC | 0.8692 |

---

# Tech Stack

## Backend Framework
- FastAPI
- Uvicorn
- REST API Architecture
- Python

## Machine Learning
- Scikit-learn
- Gradient Boosting Classifier
- Logistic Regression
- Random Forest
- AdaBoost
- Support Vector Classifier (SVC)

## Data Processing
- Pandas
- NumPy

## Data Preprocessing
- ColumnTransformer
- Pipeline Architecture
- StandardScaler
- OneHotEncoder
- SimpleImputer
- Feature Engineering

## Model Evaluation
- Cross Validation
- Stratified K-Fold
- ROC-AUC Evaluation
- Accuracy Metrics
- Precision / Recall
- F1-score
- Confusion Matrix

## Data Visualization
- Matplotlib
- Seaborn
- Heatmaps
- KDE Plots
- Violin Plots
- Pairplots
- Correlation Matrices

## Model Persistence & Serialization
- Joblib
- Pickle-based ML Pipeline Serialization

## API & Inference
- JSON-based API Requests
- Real-time ML Inference
- Probability Prediction System
- POST API Endpoints

## Backend Architecture
- Modular ML Pipeline
- Deployment-ready Inference System
- Production-style API Structure
- Automated Preprocessing Pipeline

## Deployment & Hosting
- Render
- GitHub
- Git

## Developer Tools
- VS Code
- Jupyter Notebook
- Chrome DevTools
- GitHub Version Control

## Concepts Demonstrated
- Machine Learning Workflow
- End-to-End ML Deployment
- Full Stack Integration
- Model Evaluation & Selection
- Explainable Machine Learning
- Production ML Pipeline Design
- API Development
- Responsive Frontend Integration
---

# API Endpoint

## POST `/predict`

Predict customer churn probability.

Example Request:

```json
{
  "customer_id": 123456789,
  "credit_score": 650,
  "country": "France",
  "gender": "Male",
  "age": 40,
  "tenure": 3,
  "balance": 50000,
  "products_number": 2,
  "credit_card": 1,
  "active_member": 1,
  "estimated_salary": 60000
}
```

---

## Example Response

```json
{
  "prediction": 0,
  "churn_probability": 0.03
}
```

---

# Installation

## Clone Repository

```bash
git clone https://github.com/your-username/churn-backend.git
```

---

## Install Dependencies

```bash
pip install -r requirements.txt
```

---

## Run Server

```bash
uvicorn main:app --reload
```

---

# Project Structure

```bash
backend/
│
├── main.py
├── best_churn_pipeline.pkl
├── requirements.txt
└── notebooks/
```

---

# Author

Stuti

Built using FastAPI and Machine Learning.
