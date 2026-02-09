# 🚗 Used Car Price Prediction App

🎥 Demo Video:  
https://youtu.be/RVstGS_p7r0

This project is an end-to-end Machine Learning application that predicts used car prices using structured vehicle data from Kaggle.

---

## 📌 Project Overview

The goal is to build a reliable regression model capable of estimating used car prices based on features such as mileage, engine power, brand, transmission type, fuel type, accident history, and colors.

The project covers the full ML pipeline:
- Data cleaning & preprocessing
- Feature engineering
- Outlier handling
- Model comparison
- Hyperparameter tuning
- Cross-validation
- Deployment with FastAPI

---

## 🔧 Data Processing

- Converted price and mileage to numeric format
- Extracted engine horsepower
- Created `car_age` from model year
- Simplified transmission and color categories
- Encoded fuel types (diesel, hybrid, flexfuel)
- Removed extreme price outliers (> $300,000)
- Applied log transformation to target variable

---

## 🤖 Model

Multiple models were tested:
- Linear Regression
- Ridge
- Decision Tree
- Random Forest
- LightGBM
- **XGBoost (Final Model)**

The final model is built using a full preprocessing + XGBoost pipeline.

---

## 📈 Performance

- **Cross-Validation R²:** ~0.85  
- **Test R²:** ~0.80+  
- **MAE:** ~8,000 USD  
- **RMSE:** ~15,000 USD  

---

## 🌐 Deployment

The trained model is deployed using **FastAPI** and includes:
- `/predict` endpoint
- Web-based user interface
- Real-time price estimation

---

## 🚀 Conclusion

This project demonstrates a complete ML workflow from raw dataset to deployed production-ready application, achieving strong generalization performance (~85% CV R²).

---

© Anıl Keleş
