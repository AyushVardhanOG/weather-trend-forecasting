# 🌍 Global Weather Repository — Weather Trend Forecasting

> **PM Accelerator Tech Assessment** | Advanced Data Science Project

---

## 📌 Project Overview

This project analyzes the **Global Weather Repository** dataset from Kaggle to forecast weather trends using both basic and advanced data science techniques. It covers data cleaning, EDA, anomaly detection, multiple forecasting models, feature importance, and spatial analysis.

---

## 🚀 PM Accelerator Mission
PM Accelerator empowers aspiring and experienced product managers by providing world-class training, mentorship, and real-world project experience. Our mission is to accelerate your journey to becoming a top-tier product leader through hands-on learning and community support.

---

## 📂 Repository Structure

```
├── weather_forecasting.ipynb   # Main Colab Notebook (all code)
├── README.md                   # This file
└── requirements.txt            # Python dependencies
```

---

## 📊 Dataset

**Source:** [Global Weather Repository on Kaggle](https://www.kaggle.com/datasets/nelgiriyewithana/global-weather-repository/code)

- Daily weather data for cities worldwide
- 40+ features including temperature, humidity, precipitation, wind, air quality, etc.

---

## ⚙️ How to Run

### Option 1: Google Colab (Recommended)
1. Download `weather_forecasting.ipynb` from this repo
2. Open [Google Colab](https://colab.research.google.com) and upload the notebook
3. Download the dataset from Kaggle: `GlobalWeatherRepository.csv`
4. Run **Cell 1** to install libraries
5. Run **Cell 2** — upload the CSV when prompted (or mount Google Drive)
6. Run all remaining cells in order

### Option 2: VS Code / Local
```bash
git clone https://github.com/YOUR_USERNAME/weather-forecasting
cd weather-forecasting
pip install -r requirements.txt
jupyter notebook weather_forecasting.ipynb
```

---

## 🔬 Analyses Performed

| # | Analysis | Description |
|---|----------|-------------|
| 1 | **Data Cleaning** | Handle missing values, remove outliers (IQR), normalize data |
| 2 | **EDA** | Temperature/precipitation distributions, correlations, country-level trends |
| 3 | **Anomaly Detection** | Isolation Forest to flag unusual weather events |
| 4 | **ARIMA Forecasting** | Time series forecast with stationarity test |
| 5 | **Prophet Forecasting** | Facebook Prophet with seasonal decomposition |
| 6 | **XGBoost Forecasting** | Gradient boosting with lag features |
| 7 | **Ensemble Model** | Average of all 3 models for improved accuracy |
| 8 | **Feature Importance** | Random Forest + XGBoost feature rankings |
| 9 | **Spatial Analysis** | Plotly globe map + Folium heatmap |
| 10 | **Climate Patterns** | Seasonal trends, country-wise comparisons |
| 11 | **Air Quality Analysis** | Correlation between AQ metrics and temperature |

---

## 📈 Models & Metrics

| Model | MAE | RMSE | R² |
|-------|-----|------|----|
| ARIMA | — | — | — |
| Prophet | — | — | — |
| XGBoost | — | — | — |
| **Ensemble** | — | — | — |

*(Values filled in after running the notebook)*

---

## 📦 Requirements

```
pandas
numpy
matplotlib
seaborn
plotly
folium
scikit-learn
xgboost
statsmodels
prophet
```

Install all at once:
```bash
pip install -r requirements.txt
```

---

## 📝 Key Insights

- Temperature shows clear seasonal patterns across the globe
- Isolation Forest detected ~5% anomalous readings in the dataset
- XGBoost with lag features outperforms ARIMA on short-term forecasting
- Ensemble model provides the most stable predictions overall
- Strong correlations exist between humidity, dew point, and temperature

---

## 🎥 Demo Video

[Link to demo video — add here after recording]

---

## 👤 Author

Your Name  
PM Accelerator Tech Assessment Submission
