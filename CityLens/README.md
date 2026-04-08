# 🚦 CityLens Traffic AI

> Intelligent Urban Traffic Congestion Prediction System

![Python](https://img.shields.io/badge/Python-3.9+-blue?style=flat-square&logo=python)
![Streamlit](https://img.shields.io/badge/Streamlit-1.x-red?style=flat-square&logo=streamlit)
![ML](https://img.shields.io/badge/ML-5%20Models-green?style=flat-square)
![Datasets](https://img.shields.io/badge/Datasets-3%20Real--World-orange?style=flat-square)
![License](https://img.shields.io/badge/License-MIT-purple?style=flat-square)

## 🌐 Live Demo
[CityLens Traffic AI →](https://citylens-traffic-ai.streamlit.app)

---

## 🔍 Dashboard Technical Directory

| Dashboard | Description |
|---|---|
| **🏠 Smart City Hub** | The central command center providing a high-level system overview, real-time status pulses, and quick navigation modules. |
| **🌍 Live Traffic Map** | Real-world urban intelligence dashboard. Features TomTom API integration, incident tracking, and dual-city comparison benchmarks. |
| **🔮 Live Predictor** | AI inference engine. Uses the trained Random Forest model to predict congestion levels based on vehicle counts, rain, and occupancy. |
| **📊 Analytics** | Deep-dive exploration. Interactive Plotly visuals for all 3 major traffic datasets (US Accidents, Smart Mobility, City Flow). |
| **📈 Performance** | Model evaluation studio. Displays accuracy scores, confusion matrices, and feature importance rankings for the ML ensemble. |

---

## 📌 Overview

**CityLens Traffic AI** predicts urban traffic congestion levels — **Low / Medium / High** — using 5 classical machine learning models trained on 3 real-world datasets sourced from Kaggle.

The system includes:
- A **live congestion predictor** with AI confidence scoring
- **Interactive Plotly analytics** across all 3 datasets
- **Model comparison dashboard** with confusion matrices and feature importance
- A premium **dark-theme UI** with glassmorphism, animations, and custom CSS

---

## 🚀 Features

| Feature | Description |
|---|---|
| 🔮 Live Predictor | Input road conditions and get instant ML-powered severity classification |
| 🌍 Live Traffic Map | **ULTIMATE UPGRADE**: Real-time TomTom flow & incidents, dual-city comparison, and geolocation |
| 📊 Analytics Dashboard | Deep visual analysis with Plotly charts for all 3 datasets |
| 📈 Traffic Timeline | High-fidelity Past/Future timeline with "NOW" anchor and ML forecasts |
| 🤖 AI Insight Card | Smart tactical analysis and driver recommendations generated from live road metrics |
| 🏆 Model Performance | Compare all 5 models with real accuracy, F1, AUC-ROC metrics |
| 🎨 Premium UI | Dark theme, animated cards, gradient hero, glassmorphism design |
| 🧠 5 ML Models | All trained, saved, and evaluated against real test data |

---

## 🛠️ Feature Technical Glossary

### 🌍 Live Traffic Map Dashboard

| Item | Technical Description |
|---|---|
| **🔍 Search City** | Uses `geopy (Nominatim)` to convert city names to Lat/Lng coordinates and updates the global map center. |
| **📍 City Chips** | One-tap navigation buttons for major global hubs (London, Tokyo, etc.) with pre-set coordinates. |
| **🔴 Auto Refresh** | Toggle state-based silent updates every 60 seconds. Uses TomTom API to refresh road segments without reloading the page. |
| **⚖️ Comparison Mode** | Activates a dual-pane layout. Allows you to compare real-time traffic conditions of two different cities side-by-side. |
| **🚦 Active Incidents** | Fetches data from TomTom Incident Details API. Displays delays, construction, and accidents as interactive markers. |
| **📊 Congestion Breakdown** | A Plotly-powered Donut chart summarizing the percentage of roads in Green (Free), Orange (Slow), or Red (Congested) states. |
| **📈 Traffic Timeline** | A high-fidelity chart showing the past 5 hours of traffic history and a 2-hour AI-driven forecast using congestion trends. |
| **🤖 CityLens AI** | An intelligent interpretation engine that analyzes live metrics (Speed/Delay) and produces tactical recommendations. |

---

## 🧠 Models Used

| Model | Description |
|---|---|
| ⭐ Random Forest | Ensemble tree method — best accuracy on both datasets |
| 🚀 XGBoost | Gradient boosting — high performance, fast inference |
| 📐 Support Vector Machine | Linear SVC with regularization |
| 🌳 Decision Tree | Interpretable single-tree classifier |
| 📉 Logistic Regression | Baseline linear probabilistic model |

---

## 📊 Datasets

| Dataset | Source | Records | Key Features |
|---|---|---|---|
| US Traffic Congestion 2016–2022 | Kaggle (sobhanmoosavi) | ~7 Million | Severity, Delay, Speed, Location |
| Smart Mobility Traffic Dataset | Kaggle (ziya07) | 5,000 | Vehicle Count, Speed, Occupancy, Weather |
| Traffic Prediction Dataset | Kaggle (hasibullahaman) | ~3,000 | CarCount, BikeCount, BusCount, Hour |

---

## ⚙️ Run Locally

```bash
# 1. Clone the repo
git clone https://github.com/mounibwassim/CityLens.git
cd CityLens

# 2. Install dependencies
pip install -r requirements.txt

# 3. Train all 5 models (downloads datasets from Kaggle via kagglehub)
python train_models.py

# 4. Launch the Streamlit app
streamlit run app.py
```

> **Note:** `train_models.py` will automatically download the datasets from Kaggle using `kagglehub`. No manual dataset download needed.

---

## 🛠️ Tech Stack

`Python` · `Streamlit` · `Scikit-learn` · `XGBoost` · `Plotly` · `Pandas` · `NumPy` · `KaggleHub` · `Joblib`

---

## 📁 Project Structure

```
CityLens-Traffic-AI/
│   app.py                  ← Main Streamlit dashboard
│   train_models.py         ← Training pipeline (all 5 models × 2 datasets)
│   requirements.txt        ← Dependencies for deployment
│   README.md
│   .gitignore
│
├── assets/                 ← Real-life imagery for each page
│   ├── smart_city_home.png
│   ├── live_predictor_bg.png
│   ├── traffic_analytics.png
│   ├── model_performance_ai.png
│   └── about_citylens.png
│
└── models/                 ← Generated after running train_models.py
    ├── random_forest_ds2.joblib
    ├── xgboost_ds2.joblib
    └── ...
```

---

## 🤝 Contributors

Built with ❤️ for Smart City Innovation · **CityLens Traffic AI © 2026**
