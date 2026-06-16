# Global Weather Repository — Weather Trend Forecasting
**PM Accelerator Tech Assessment**

---

## PM Accelerator Mission

Welcome to PM Accelerator, a beacon of guidance for aspiring and experienced PMs alike. We have designed this platform to offer training, education, and job opportunities for Product Managers, creating room for constant improvement and shaping the next generation of PMs.

**Our Mission:** By making industry-leading tools and education available to individuals from all backgrounds, we level the playing field for future PM leaders. We grant aspiring and experienced PMs what they need most — Access.

---

## Project Overview

This project analyzes the **Global Weather Repository** dataset from Kaggle to forecast global weather trends. It covers data cleaning, exploratory data analysis, anomaly detection, multiple forecasting models, feature importance, air quality analysis, and spatial/climate pattern analysis.

**Dataset:** [Global Weather Repository — Kaggle](https://www.kaggle.com/datasets/nelgiriyewithana/global-weather-repository)

---

## Results

| Metric | Value |
|--------|-------|
| Raw Dataset | 146,760 rows × 41 features |
| After Cleaning | 144,301 rows |
| Date Range | May 2024 – June 2026 |
| Target Variable | temperature_celsius |
| Mean Temperature | 21.74°C (range: -2.0 to 45.8°C) |
| Anomalies Detected | 7,215 (5%) via Isolation Forest |
| Best Model | XGBoost — MAE: 0.414 · RMSE: 1.226 · R²: 0.681 |

### Model Comparison

| Model | MAE | RMSE | R² |
|-------|-----|------|----|
| ARIMA (5,1,0) | 1.5763 | 2.3601 | -0.1954 |
| Prophet | 2.0716 | 2.5376 | -0.3819 |
| **XGBoost** | **0.4139** | **1.2258** | **0.6811** |
| Ensemble | 0.6548 | 1.3554 | 0.5972 |

---

## Analyses Performed

| Analysis | Method | Key Finding |
|----------|--------|-------------|
| Data Cleaning | IQR + StandardScaler | 0 missing values; 2,459 outliers removed |
| EDA | Distributions, Correlations | 8°C seasonal range; humidity negatively correlated |
| Anomaly Detection | Isolation Forest (5%) | 7,215 anomalies — extreme events & sensor noise |
| Forecasting | ARIMA, Prophet, XGBoost, Ensemble | XGBoost best; lag features key signal |
| Feature Importance | Random Forest + XGBoost | feels_like_celsius most predictive (38.2%) |
| Spatial Analysis | Plotly globe + Folium heatmap | Equatorial regions hottest |
| Air Quality | Correlation analysis | UV↔Ozone (0.71); rain reduces PM10 |

---

## Key Insights

- XGBoost with lag features is the best model — yesterday's temperature is the strongest predictor
- Linear models (ARIMA, Prophet) underperform on globally aggregated weather data
- 5% of readings are anomalous — traced to extreme heat events, dust storms, or sensor noise
- Air quality is strongly weather-dependent — UV drives ozone, rain clears particulates
- Clear seasonal pattern: 8°C range from December trough to July peak

---

## Files

| File | Description |
|------|-------------|
| `weather_forecasting.ipynb` | Full Colab notebook with all code and outputs |
| `Weather_Forecasting_Report.docx` | Complete project report |
| `requirements.txt` | Python dependencies |

---

## Demo Video

[Add demo video link here]

---

*Submitted for PM Accelerator Tech Assessment — June 2026*
