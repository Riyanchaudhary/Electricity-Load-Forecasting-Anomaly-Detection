# AI-Based Power Load Forecasting & Anomaly Detection

A machine learning system that forecasts electricity demand and detects
anomalies in power usage using real-world hourly energy data from the
PJM East region.

---

## Overview

Utilities and energy managers need reliable demand forecasts and early
warning systems for irregular consumption. This project addresses both:
- **Load Forecasting** — predict future electricity demand from temporal features
- **Anomaly Detection** — flag unexpected spikes or drops in consumption

---

## Tech Stack

- **Python**, Pandas, Scikit-learn, Matplotlib
- **RandomForestRegressor** — load forecasting
- **IsolationForest** — anomaly detection

---

## Dataset

- **Source:** PJM Energy (publicly available)
- **Type:** Hourly electricity load data, PJM East region
- **Usage:** Model training, validation, anomaly detection

---

## Pipeline

1. **Load & Clean** — remove nulls, parse timestamps
2. **Feature Engineering** — extract hour, day, weekday
3. **Forecasting** — train RandomForestRegressor, evaluate with MAE
4. **Anomaly Detection** — IsolationForest flags irregular consumption
5. **Visualization** — actual vs predicted plot + anomaly timeline

---

## Results

| Metric | Value |
|--------|-------|
| MAE | ~3000 MW |
| Error Rate | ~12% |

---

## Visualizations

- **Actual vs Predicted Load** — tracks model accuracy over time
- **Anomaly Timeline** — red markers highlight flagged anomalies

---

## Author

Riyan Chaudhary
