🚦 Traffic Risk Prediction System
🧠 Android App + Machine Learning Backend
<p align="center"> <img src="https://img.shields.io/badge/Android-Java%20%7C%20Kotlin-brightgreen?logo=android&style=for-the-badge" /> <img src="https://img.shields.io/badge/Backend-Python%20%7C%20Flask-blue?style=for-the-badge&logo=python" /> <img src="https://img.shields.io/badge/ML-ScikitLearn-orange?style=for-the-badge&logo=scikitlearn" /> <img src="https://img.shields.io/badge/Platform-Mobile%20%7C%20API-purple?style=for-the-badge" /> </p>

A complete Traffic Accident Risk Prediction System consisting of:

✔ Android application for user inputs
✔ Machine-learning backend API
✔ Real-time accident risk prediction
✔ Clean UI + optimized model pipeline

📱 Android App: Traffic Risk Predict App

The Android application collects user data such as weather, road type, traffic density, and driver conditions, then communicates with the backend API to predict the accident risk level.

🚀 Features

Modern Material UI

Retrofit2 API integration

Java/Kotlin clean code

Form validation before prediction

Real-time risk prediction with severity UI

Optimized for low-end devices

🏗 Tech Stack

Java / Kotlin

Retrofit2

Material Design Components

MVVM (optional, if implemented)

Android Studio

📦 Android Project Structure
Android App/
└── Traffic_RiskPredictApp
    ├── app
    ├── build
    ├── gradle
    ├── build.gradle
    ├── settings.gradle
    └── local.properties

🔌 API Integration Example

Endpoint:

POST /predict
Content-Type: application/json


Sample Request:

{
  "Weather": "Sunny",
  "Road_Type": "Highway",
  "Time_of_Day": "Day",
  "Traffic_Density": 2,
  "Speed_Limit": 80,
  "Number_of_Vehicles": 3,
  "Driver_Alcohol": 0,
  "Road_Condition": "Dry",
  "Vehicle_Type": "Car",
  "Driver_Age": 28
}

🧠 ML Backend — Traffic Risk Prediction API

The backend contains a full machine-learning pipeline for predicting traffic accident severity.

🚀 Backend Features

Complete ML training pipeline

Preprocessing with saved transformer

Model training + evaluation

Clean JSON prediction output

Flask / FastAPI endpoint

Ready-to-deploy on Render / Railway

🏗 Backend Structure
Traffic_risk_prediction Backend/
 ├── app.py                 # API Endpoint
 ├── predict.py             # Prediction logic
 ├── train.py               # Model training
 ├── data_process.py        # Cleaning & preprocessing
 ├── preprocessor.pkl       # Preprocessing pipeline
 ├── trained_model.pkl      # ML model
 ├── dataset_traffic_accident_prediction1.csv
 ├── evaluation_metrics.json
 ├── requirements.txt
 └── render.yaml            # Cloud deployment config

🔬 ML Workflow
1️⃣ data_process.py

Clean dataset

Handle missing values

Encode categorical features

2️⃣ train.py

Train ML model

Save:
✔ trained_model.pkl
✔ preprocessor.pkl

3️⃣ predict.py

Loads model & preprocessor

Prepares input

Returns predicted risk level

4️⃣ app.py

Exposes /predict API endpoint

🌐 API Output Example

Response:

{
  "risk_level": "Medium",
  "confidence": 0.78
}

🛠 Installation Guide
📱 Android App

Clone repository

Open in Android Studio

Set API URL in Retrofit:

BASE_URL = "http://<your-backend-url>";


Run app on emulator or device

🧠 Backend Setup
1️⃣ Create Virtual Environment
python -m venv venv
venv\Scripts\activate     # Windows
source venv/bin/activate  # Mac/Linux

2️⃣ Install Requirements
pip install -r requirements.txt

3️⃣ Run API Server
python app.py

🚀 Deployment (Render / Railway)
Already included: render.yaml

Steps:

Push repo to GitHub

Create New Web Service on Render

Select Python runtime

Render auto-detects config

Deploy 🎉

📈 Evaluation Metrics Example
{
  "accuracy": 0.87,
  "precision": 0.82,
  "recall": 0.80,
  "f1_score": 0.81
}


🤝 Contributing

Pull requests are welcome!
Feel free to suggest improvements for UI, model, or API.

📜 License

This project is licensed under MIT License.
