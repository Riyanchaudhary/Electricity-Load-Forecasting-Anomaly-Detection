🔌 AI-Based Power Load Forecasting & Anomaly Detection
This project leverages machine learning to predict future electricity demand and detect anomalies (like unexpected spikes or drops) in power usage. Built using Python and real-world energy data, it offers actionable insights for energy management and utility planning.

📌 What It Does
🔮 Forecasts electricity load based on:

Time of day

Date

Weekday

🌲 Trains a Random Forest model to predict demand with around 12% error.

⚠️ Detects anomalies in electricity usage using Isolation Forest — useful for spotting power outages, misuse, or irregular consumption.

📈 Visualizes results through:

Actual vs. Predicted Load graph

Anomaly Detection timeline with red markers

🧠 Tech Behind It
Python – Core programming language

Pandas – Data preprocessing & feature extraction

Matplotlib – Clean and informative graphs

Scikit-learn –

RandomForestRegressor for load forecasting

IsolationForest for anomaly detection

📊 Dataset Info
Source: PJM Energy

Type: Hourly electricity load data (PJM East region)

Used For:

Training the ML models

Validating predictions and anomaly detection

💻 How It Works
Load & Clean Data

Removes missing values

Converts timestamps into usable formats

Feature Engineering

Extracts hour, day, and weekday from timestamps

Model Training

Trains a RandomForestRegressor on historical load data

Evaluates performance using Mean Absolute Error (MAE)

Achieved ~3000 MW MAE → approx. 12% error

Anomaly Detection

Uses IsolationForest to flag unusual behavior in load data

Visualization

Plots predictions vs. actual load

Highlights anomalies with red dots for interpretability

📈 Sample Results
MAE: ~3000 MW

Error: ~12%

📉 Actual vs Predicted Load Over Time
![image](https://github.com/user-attachments/assets/87ec1a95-6b9f-482b-a0fa-d100f2675339)


🔴 Anomalies on a Timeline Graph
![image](https://github.com/user-attachments/assets/3418be24-1ff3-46b5-aa8f-7f60a86052ab)



📊 Graphs Explained
1. Actual vs Predicted Load Graph
Purpose: Compare model predictions against true values

Insights:

Small gaps = accurate model

Large gaps = areas of error

Observation:

Predictions align well with actuals → only ~12% average error

2. Anomaly Detection Graph
Purpose: Spot unusual consumption patterns over time

Highlights:

Red dots indicate flagged anomalies

Helps detect possible system faults or unexpected usage

📌 Example Scenarios
⚡ A spike at midnight → May indicate equipment failure or reporting error

⚡ Drop during peak hours → Could signal outages or sensor malfunctions
