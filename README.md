# **Multi-Energy-Analysis-and-Forecasting-for-Building-Energy-Efficiency_Part1**
### **Project Overview**
This repository presents the first part of a two-phase project on **energy efficiency in buildings**.
The goal is to explore, analyze, and model building energy consumption using a labeled dataset (with measured electricity, chilled water, steam, and hot water usage).
This stage focuses on **data exploration, cleaning, feature engineering, and predictive modeling** to better understand the drivers of energy use and provide interpretable insights for sustainable energy management.

### **Objectives**

#### **1. Data Preparation**
* Import datasets and convert energy units.
* Handle missing values and outliers.
* Prepare consistent train/test datasets.

#### **2. Feature Engineering**
* Create **time-based features** (hour, day, season).
* Add **weather interaction features** (temperature × occupancy).
* Engineer building-level attributes (age, area, use type).

#### **3. Exploratory Data Analysis (EDA)**
* Explore target variable distributions.
* Study **temporal patterns** (daily, weekly, seasonal).
* Analyze **building-level differences** in consumption.
* Evaluate **weather impact** on energy use.

#### **4. Modeling Energy Density**
* Train **separate models for each energy type** (electricity, chilled water, steam, hot water).
* Use **LightGBM (LGBMRegressor)** with IQR outlier handling.
* Compare model performance across energy types.

#### **5. Interpretation & Visualization**
* Feature importance ranking.
* **SHAP values** for global & local interpretability.
* Residual analysis and error distribution.
* Error breakdown by **building, time, and weather factors**.

### **Tech Stack**
* **Python** (pandas, numpy, scikit-learn, matplotlib, seaborn)
* **LightGBM** for regression modeling
* **SHAP** for model interpretability
* **Jupyter Notebooks** for exploration & analysis

### **Key Results**
* Clear temporal and weather-driven patterns in building energy use.
* Distinct drivers identified for each energy type.
* LightGBM models achieve strong predictive performance with interpretable drivers.
* SHAP analysis highlights **temperature, building use, and occupancy patterns** as major factors.

### **Next Steps (Part 2)**

The second phase will use the **unlabeled dataset** for:
* Forecasting energy consumption under different scenarios.
* Efficiency tracking over time.
* Anomaly detection (faults, waste, data errors).
* Portfolio-level insights for predictive control & sustainability.

### **Contributions**

Contributions, suggestions, and discussions are welcome! Please open an issue or pull request.
