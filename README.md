# ALF Risk Prediction

This project predicts next-day health incident risk for Assisted Living Facility (ALF) residents using synthetic data.

## 🔍 Overview

Each day, caregivers log basic health data for each resident. This model uses recent vitals and trends to identify high-risk patients so facility staff can proactively intervene.

## 📁 Project Structure

```
alf_risk_prediction/
├── data/                # Synthetic dataset (CSV)
├── notebooks/           # Jupyter Notebooks (EDA, Modeling, etc.)
├── reports/             # Summary reports, documentation
├── figures/             # Plots and visualizations
├── src/                 # Source code (modeling, preprocessing)
└── README.md            # Project description
```

## 📈 Key Features

- Synthetic daily health logs for 200 residents across 30 days
- Engineered features like vital sign changes, age groups
- Trained a Random Forest model with performance ~0.83 ROC AUC
- Top predictors: medication adherence, heart rate variability, BP changes

## 📊 Usage

1. Clone this repo
2. Explore `notebooks/` for EDA and modeling
3. Review `reports/summary.md` and `figures/` for key insights

## 🧠 Future Work

- Real-time monitoring integration
- Time-series or sequence modeling (e.g., LSTM)
- Expanded features (sleep, mobility, cognition)
