# ✈️ Flight Delay Prediction using Machine Learning

Predicting flight delays using large-scale aviation data and machine learning models.

## 📌 Overview

Flight delays cost the aviation industry billions and inconvenience millions of travelers every year. This project aims to **predict whether a flight will be delayed** using historical flight data, weather information, and airline details.

The project involves:
- Building multiple ML models to classify flight delay occurrences
- Creating a web interface for data upload and predictions
- Visualizing insights and performance metrics

---

## 🚀 Features

- ✅ Delay prediction using real flight data
- 📊 Data preprocessing, feature encoding, and visualizations
- 🔍 ML models used: Random Forest, SVM, LSTM (for comparison)
- 🌐 Flask web application for interaction and real-time prediction
- 📈 Accuracy: ~87% with Random Forest on binary classification

---

## 🛠️ Tech Stack

- **Language:** Python 3.8+
- **Libraries & Frameworks:**  
  - `scikit-learn`, `pandas`, `numpy`, `matplotlib`, `seaborn`  
  - `Flask` for web application  
  - `joblib` for model saving/loading  
  - `LabelEncoder`, `RandomForestClassifier`  
- **Databases:** MongoDB, PostgreSQL
- **Deployment:** Localhost via PyCharm IDE

---

## 📂 Dataset

- Historical flight data including:
  - Airline
  - Origin and Destination airports
  - Scheduled departure/arrival time
  - Delay status (target variable)
- Additional datasets:
  - `planes.csv`, `airports.csv`, `carriers.csv`

---

## 📊 Model Performance

| Model          | Accuracy |
|----------------|----------|
| Random Forest  | **87%**  |
| SVM            | ~78%     |
| LSTM (limited) | ~75%     |

> Random Forest gave the best performance without overfitting and with high generalization.

---

## 🧪 How to Run Locally

1. **Clone the repository:**
   ```bash
   git clone https://github.com/MudassirMubeen/flight-delay-prediction.git
   cd flight-delay-prediction

flight-delay-prediction/
│
├── app.py                        # Main Flask application
├── create_model.py              # Model training and saving script
├── predict.py                   # Prediction logic
├── preprocess.py                # Data cleaning and preprocessing
├── requirements.txt             # Python dependencies
├── README.md                    # Project overview (you already have this)
├── LICENSE                      # Optional: MIT or other license
│
├── 📁 static/                   # Static files (CSS, JS, images)
│   └── styles.css               # Optional: custom styles for frontend
│
├── 📁 templates/                # HTML templates (for Flask)
│   ├── index.html               # Home page
│   ├── admin_login.html         # Admin login
│   ├── user_login.html          # User login
│   ├── predict.html             # Prediction page
│   ├── results.html             # Display prediction result
│   └── upload.html              # Upload dataset UI
│
├── 📁 models/                   # Trained models
│   └── Flight_RF.pkl            # Pickled Random Forest model
│
├── 📁 data/                     # Datasets (raw or processed)
│   ├── flight_data.csv
│   ├── airports.csv
│   ├── planes.csv
│   ├── carriers.csv
│   └── processed_data.csv
│
├── 📁 screenshots/              # UI screenshots for README
│   ├── admin.png
│   └── predict.png
│
└── 📁 utils/                    # Helper functions and utilities
    └── visualization.py        # Code for graphs/charts
