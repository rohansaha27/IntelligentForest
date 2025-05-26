# 🔥 Intelligent Forest: Predicting Wildfire Risk with AI

This project leverages machine learning to predict the risk level of forest fires using local climate data. It focuses on the Brisbane, Queensland region and uses historical fire alerts and weather data to classify daily fire risk as **No Risk, Low Risk, Medium Risk, or High Risk**.

---

## 🌍 Problem Statement

Climate change has increased the frequency and severity of forest fires. As wildfires threaten ecosystems globally, early prediction and prevention is critical. This project aims to build an AI model that can assess the likelihood of forest fires in a given region based on a few key weather conditions.

---

## 📊 Data Sources

- **Fire Alerts (2012–2022)**: Collected from [Global Forest Watch](https://www.globalforestwatch.org), based on VIIRS satellite alerts.
- **Climate Data**: Weather features including temperature, humidity, and evaporation sourced from [Kaggle's Rattle Weather Dataset](https://www.kaggle.com/datasets/jsphyg/weather-dataset-rattle-package).

### Features Used:
- Minimum Temperature (°C)
- Maximum Temperature (°C)
- Rainfall (mm)
- Solar Radiation (MJ/m²)
- Evaporation (mm)

---

## 🧠 Models & Methodology

We trained two models to predict fire risk using supervised learning techniques:

- 🌳 **Decision Tree**
  - Accuracy: 70%
- 🌲 **Random Forest**
  - Accuracy: 79%

Both models were trained on historical climate + fire data and tested using confusion matrices to assess prediction reliability.

---

## 📁 Project Structure

```bash
.
├── data/
│   ├── climate_data.csv
│   └── fire_alerts.csv
├── notebooks/
│   ├── data_cleaning.ipynb
│   └── model_training.ipynb
├── src/
│   ├── preprocess.py
│   └── model.py
├── results/
│   ├── decision_tree_confusion_matrix.png
│   └── random_forest_confusion_matrix.png
└── README.md
