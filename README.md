📊 Bengaluru Traffic Forecasting (2022–2024)

Time Series Analysis – Classical + Advanced Forecasting Models

This project builds a complete end-to-end Time Series Forecasting pipeline to predict hourly/daily traffic volume for Bengaluru (2022–2024).
It strictly follows the academic TSA Phase-1 (Classical Validation) and Phase-2 (Advanced Forecasting) workflow.

🚀 Key Outcomes

Cleaned & aggregated hourly → daily traffic dataset

Rolling means, decomposition, seasonality extraction

SARIMA & Holt-Winters forecasting

14-day & 30-day future traffic predictions

Full model comparison (RMSE, MAE, MAPE)

Exported plots + metrics + processed datasets

📁 Project Structure
bengaluru-traffic-forecasting-tsa/
│
│  Phase1&2_TSA.ipynb            # Main TSA notebook
│  requirements.txt               # Dependencies
│  README.md                      # Documentation
│
├── data/
│     └── Banglore_traffic_Dataset.csv
│
└── ts_phase_outputs/
      ├── traffic_daily_cleaned.csv
      ├── forecast_14d.csv
      ├── forecast_30d.csv
      ├── models_metrics.csv
      └── plots/
           ├── forecast_14d.png
           └── rolling.png

🧪 Phase-1: Classical TSA Workflow
✔ 1. Dataset Overview

Hourly traffic volume (Jan 2022 → Dec 2024)

Converted to daily totals

No missing timestamp gaps post-cleaning

✔ 2. Preliminary Analysis

Missing-value imputation

Outlier checks

Hourly & daily trend plots

Summary statistics

✔ 3. Model Structure Selection

Additive vs Multiplicative tested

Additive decomposition chosen (seasonal amplitude stable)

✔ 4. Components Extracted

Trend

Weekly seasonality

Residual series

✔ 5. Diagnostics

ADF test (stationarity)

Ljung-Box (white noise check)

ACF & PACF analysis

🎯 Phase-1 Conclusion

Clean dataset, clear weekly pattern, additive model fits → ready for SARIMA/Holt-Winters.

🚀 Phase-2: Advanced Modeling
✔ 1. SARIMA

Auto-tuned using AIC optimization

Evaluated via RMSE, MAE, MAPE

14-day and 30-day forecasts generated

✔ 2. Holt-Winters

Additive trend + seasonality

Compared head-to-head against SARIMA

✔ 3. Forecast Outputs

Stored in ts_phase_outputs/:

forecast_14d.csv

forecast_30d.csv

Plot files under /plots/

✔ 4. Model Comparison

models_metrics.csv includes:

RMSE

MAE

MAPE

Best-performing model

🔧 Installation
1️⃣ Clone Repo
git clone https://github.com/<your-username>/bengaluru-traffic-forecasting-tsa.git
cd bengaluru-traffic-forecasting-tsa

2️⃣ Install Dependencies
pip install -r requirements.txt

3️⃣ Run Notebook
jupyter notebook Phase1&2_TSA.ipynb

📦 Requirements

Used libraries:

pandas

numpy

matplotlib

seaborn

statsmodels

pmdarima

🎯 Skills Demonstrated

Time Series preprocessing

Trend / seasonality decomposition

ACF–PACF interpretation

SARIMA modeling

Holt-Winters smoothing

Hyperparameter tuning

Multi-step forecasting

RMSE / MAE / MAPE evaluation

Full TSA pipeline engineering

🌍 SDG Mapping

SDG 11 – Sustainable Cities & Communities
Traffic forecasting supports better planning, congestion control, and mobility optimization.

👤 Author

KumaraSwamy G (kay_yagamine)
AI/ML Engineering Student – BMS College of Engineering

⭐ Support

If you find this project useful, consider starring the repository!
