# SepsisX - Early Sepsis Detection System

SepsisX is a full-stack AI-powered platform for early detection of sepsis using patient vitals, lab results, and medical history. It integrates an Artificial Neural Network (ANN) or XGBoost model with a Flask backend to predict sepsis risk scores and recommend treatments. Designed for hospitals, SepsisX supports real-time monitoring, patient dashboards, risk visualization, and EHR integration via SMART on FHIR.

---

## 🚀 Features

- ✅ Predict sepsis risk using vitals and lab values
- ✅ Risk severity scoring with animated risk bars
- ✅ Treatment suggestions and lab test recommendations
- ✅ Preventive measures if risk is low
- ✅ REST API and JSON responses for integration
- ✅ Clean, responsive frontend UI (HTML/CSS/JS)
- ✅ Flask backend with trained model integration
- ✅ Role-based dashboards (Doctor, Admin, Patient)
- ✅ Deployable via Google Cloud Run, Render, or Vercel

---

## 🔧 Folder Structure

SEPSIS_PROJECT/ 
├── .dist/ # (Build folder or optional use) 
├── static/ 
│ └── style.css # Custom CSS for frontend styling
├── templates/ 
│ ├── home.html # Homepage UI 
│ ├── login.html # Login page 
│ ├── predict.html # Prediction form and results 
│ └── signup.html # Signup/registration page 
├── app.py # Main Flask application 
├── model.py # ML model loader & prediction functions 
├── Patients_Files_Train.csv # Training dataset 
├── Patients_Files_Test.csv # Test dataset 
├── scaler.pkl # Pre-fitted data scaler 
├── sepsis_model.h5 # Trained model (Keras) 
├── users.db # SQLite database for login/signup 
├── requirements.txt # Python dependencies 
└── Readme # This README file


---

## 🧪 Features

- Predict sepsis risk from patient lab/vital inputs
- ANN model trained with `.h5` file
- Frontend with login, signup, and prediction UI
- Flask backend for form handling and ML inference
- SQLite-based user authentication

---

## 📦 Installation

2. Set Up Virtual Environment

python -m venv venv
source venv/bin/activate     # On Windows: venv\Scripts\activate

3. Install Required Packages

pip install -r requirements.txt

🚀 Run the App

python app.py
The app runs at http://127.0.0.1:5000

Use the login or signup page to enter

now i Have Login details 

username -- ajay
password -- Ajay

Navigate to prediction form and test patient inputs

⚙️ File Descriptions

File	Description
app.py   	                Flask server that manages routes, sessions, and app launch
model.py	                Loads scaler and trained model, performs predictions
Patients_Files_Train.csv	Training dataset (used offline)
Patients_Files_Test.csv  	Test dataset for evaluation
sepsis_model.h5	            Trained ANN model saved using Keras
scaler.pkl	                Preprocessing scaler (used before feeding data to model)
users.db	                SQLite database with registered users
requirements.txt	        All Python packages used
templates/	                All HTML pages rendered by Flask
static/style.css	        Custom styles for UI layout

📊 Sample Input Format (CSV)

PL,PR,SK,TS,M11,BD2,Age,Insurance
5.1,120,2.3,6.7,24.5,4.2,45,1

🧪 Test & Predict
Test patients via predict.html form

Model runs inference with model.py

Results include sepsis risk score and risk status

✅ Requirements

Flask
numpy
pandas
scikit-learn
tensorflow
joblib


pip install -t requirements.txt


📤 Deployment

🔹 Google Cloud Run


📄 License
This project is open-source under the MIT License.

👩‍💻 Contributors
[Ajay kumar T N and Adithya N Murthy] --->   Model training & backend

[Manikya C S and Manoj S R] --->  Frontend & Flask routes


---
