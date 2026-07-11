# Predicting Flue Gas Emissions and Turbine Energy Yield

A machine learning project that predicts **Carbon Monoxide (CO)** emissions, **Nitrogen Oxides (NOx)** emissions, and **Turbine Energy Yield (TEY)** using operational gas turbine sensor data.

---

## Project Overview

Gas turbines are widely used for power generation, but their efficiency and emissions depend on several operating conditions. This project applies machine learning techniques to analyze turbine sensor data and accurately predict:

- Carbon Monoxide (CO)
- Nitrogen Oxides (NOx)
- Turbine Energy Yield (TEY)

The project also compares several machine learning algorithms and studies feature importance to understand which operational parameters have the greatest influence.

---

## Dataset

The dataset contains hourly gas turbine sensor measurements collected between **2011 and 2015**.

Input features include:

- Ambient Temperature (AT)
- Ambient Pressure (AP)
- Ambient Humidity (AH)
- Air Filter Difference Pressure (AFDP)
- Gas Turbine Exhaust Pressure (GTEP)
- Turbine Inlet Temperature (TIT)
- Turbine After Temperature (TAT)
- Compressor Discharge Pressure (CDP)

Target variables:

- Carbon Monoxide (CO)
- Nitrogen Oxides (NOx)
- Turbine Energy Yield (TEY)

---

## Project Pipeline

```
Load Data
      │
      ▼
Exploratory Data Analysis
      │
      ▼
Data Cleaning
      │
      ▼
Log Transformation
      │
      ▼
Feature Scaling
      │
      ▼
PCA + UMAP
      │
      ▼
Model Training
      │
      ▼
Performance Evaluation
      │
      ▼
Feature Importance Analysis
```

---

## Models Used

- Linear Regression
- Random Forest Regressor
- Support Vector Regressor (SVR)
- LightGBM
- CatBoost
- Multi-layer Perceptron (Neural Network)

---

## Feature Engineering

- Log Transformation
- StandardScaler
- Principal Component Analysis (PCA)
- UMAP

---

## Evaluation Metrics

- Mean Absolute Error (MAE)
- Root Mean Squared Error (RMSE)
- R² Score

---

## Results

Random Forest consistently achieved the best performance across the prediction tasks.

Highlights:

- Accurate prediction of CO emissions
- Accurate prediction of NOx emissions
- Accurate prediction of Turbine Energy Yield
- Feature importance analysis using Random Forest and LightGBM

---

## Repository Structure

```
.
├── README.md
├── requirements.txt
├── gas_turbine_prediction.ipynb
├── Report.pdf
├── gt_2011.csv
├── gt_2012.csv
├── gt_2013.csv
├── gt_2014.csv
└── gt_2015.csv
```

---

## Installation

Clone the repository

```bash
git clone https://github.com/rishu023/Flue_gas_emission_prediction
```

Install dependencies

```bash
pip install -r requirements.txt
```

Launch Jupyter Notebook

```bash
jupyter notebook
```

Open

```
gas_turbine_prediction.ipynb
```

---

## Technologies Used

- Python
- Pandas
- NumPy
- Scikit-learn
- LightGBM
- CatBoost
- UMAP
- Plotly
- Matplotlib
- Seaborn

---

## Future Improvements

- XGBoost implementation
- Hyperparameter tuning
- SHAP Explainability
- Deep Learning models
- Streamlit dashboard for deployment

---

## Author

**Rishu Bhadani**

IIT Bombay

B.Tech Mechanical Engineering

Minor in Artificial Intelligence and Data Science
