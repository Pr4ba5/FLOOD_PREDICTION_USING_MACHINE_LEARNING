# 🌊 Flood Risk Prediction System using Machine Learning

A real-world disaster management project that uses machine learning to predict flood risk based on weather and river data. This system classifies flood risk into **Low**, **Mid**, or **High**, helping to inform early warning systems and disaster response.

---

## 📌 Project Highlights

- ✅ Trained on real environmental data with rainfall, discharge, temperature, and seasonal variables
- ✅ Classification model using `RandomForestClassifier`
- ✅ Feature engineering includes lag variables and rolling averages
- ✅ Parallelized model training and benchmarking
- ✅ Accurate and explainable predictions with risk levels
- ✅ Designed for real-time deployment and alerts

---

## 🧠 Problem Context

Floods are one of the most frequent and devastating disasters, especially in countries like **Nepal**, where monsoon seasons and topography increase the risk. This system aims to support **early flood detection** by learning patterns from historical and real-time data.

---

## 🗃️ Dataset Overview

- Environmental variables: precipitation, temperature, humidity, pressure, river discharge, etc.
- Engineered features: lagged and rolling means over 7-day windows
- Target variables: `Flood_probability` (regression) and `Flood_risk` (classified into Low/Mid/High)

---

## 🧪 Machine Learning Pipeline

- **Preprocessing:** Handling missing values, date parsing, normalization
- **Feature Engineering:** Lagged values, mean discharge/precipitation, monsoon flags
- **Model:** `RandomForestClassifier` (`n_jobs=-1` for parallel training)
- **Evaluation:** Accuracy, Confusion Matrix, Classification Report, Latency
- **Cross-Validation:** K-Fold with serial vs parallel benchmarking

---

## ⚙️ System Architecture

```text
[Sensor/API Data] → [Preprocessing] → [ML Model Inference] → [Risk Classification] → [Alert/Dashboard]
