# ALF Risk Prediction

This project predicts next-day health incident risk for Assisted Living Facility (ALF) residents using synthetic data.

## 🔍 Overview

Each day, caregivers log basic health data for each resident. This model uses recent vitals and trends to identify high-risk patients so facility staff can proactively intervene.

## 📁 Repository Contents

| File/Folder | Description |
|-------------|-------------|
| `.gitignore` | Git ignore rules |
| `00_data_generation.ipynb` | Jupyter notebook for generating synthetic health data |
| `01_explore_and_model.ipynb` | Notebook for data exploration and model training |
| `README.md` | Project overview and usage instructions |
| `data/` | Placeholder directory for datasets |
| `feature_importance.png` | Visualization of top predictive features |
| `requirements.txt` | List of required Python packages |
| `summary.md` | Markdown summary of key findings and recommendations |
| `synthetic_alf_data.csv` | Generated synthetic dataset (200 patients × 30 days) |

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
