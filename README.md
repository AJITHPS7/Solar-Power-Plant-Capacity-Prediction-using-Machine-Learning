# Solar-Power-Plant-Capacity-Prediction-using-Machine-Learning
This project focuses on predicting the **DC Capacity (dc_capacity_kW)** of solar power plants using Machine Learning techniques.  The objective is to build a regression model that can estimate the capacity of a solar installation based on various plant characteristics, location details, system parameters, and operational information.

# ☀️ Solar Power Plant Capacity Prediction using Machine Learning

![Python](https://img.shields.io/badge/Python-3.x-blue)
![Machine Learning](https://img.shields.io/badge/Machine%20Learning-Regression-orange)
![Scikit Learn](https://img.shields.io/badge/Scikit--Learn-ML-green)
![XGBoost](https://img.shields.io/badge/XGBoost-Model-red)

---

## 📌 Project Overview

This project focuses on predicting the **DC Capacity (dc_capacity_kW)** of solar power plants using Machine Learning techniques.

The objective is to build a regression model that can estimate the capacity of a solar installation based on various plant characteristics, location details, system parameters, and operational information.

The project covers the complete Machine Learning workflow:

**Data Collection → Data Cleaning → Exploratory Data Analysis → Feature Engineering → Model Training → Hyperparameter Optimization → Evaluation**

---

# 🎯 Problem Statement

Solar power generation depends on multiple factors such as:

- Location
- Plant configuration
- System specifications
- Tracking mechanism
- Environmental conditions

Accurate capacity estimation helps in:

- Solar project planning
- Performance analysis
- Energy forecasting
- Renewable energy optimization

---

# 📂 Dataset Description

The dataset contains solar power plant information including:

| Feature | Description |
|---|---|
| system_id | Unique plant identifier |
| location | Plant location |
| latitude | Geographic latitude |
| longitude | Geographic longitude |
| tracking | Tracking system information |
| system_size | Solar system size |
| dc_capacity_kW | Target variable |

Target:

```
dc_capacity_kW
```

---

# 🏗️ Machine Learning Pipeline

```
Dataset
   |
   |
Data Cleaning
   |
   |
Exploratory Data Analysis
   |
   |
Feature Engineering
   |
   |
Train/Test Split
   |
   |
Model Training
   |
   |
Evaluation
   |
   |
Best Model Selection
```

---

# 🧹 Data Preprocessing

Performed preprocessing steps:

✅ Removed unnecessary columns

Removed:

- IDs
- Names
- Timestamp fields
- Empty columns
- Metadata columns


Example:

```
system_id
system_public_name
first_timestamp
last_timestamp
```

---

## Missing Value Handling

Numeric columns:

```
Median Imputation
```

Categorical columns:

```
Mode Imputation
```

---

## Feature Encoding

Categorical variables were converted into numerical values using:

- Label Encoding
- One Hot Encoding

---

# 📊 Exploratory Data Analysis

Performed visual analysis:

## DC Capacity Distribution

Analyzed the distribution of solar plant capacity.

---

## Location Analysis

Studied relationship between:

```
Latitude vs DC Capacity
```

---

## Correlation Analysis

Generated correlation matrix to understand feature relationships.

---

## Tracking System Analysis

Compared capacity variation based on tracking technology.

---

# 🤖 Machine Learning Models Used

## 1. Random Forest Regressor

Random Forest combines multiple decision trees to improve prediction accuracy.

Advantages:

- Handles nonlinear relationships
- Reduces overfitting
- Works well with tabular data


---

## 2. Gradient Boosting Regressor

Gradient Boosting builds models sequentially to reduce prediction errors.

Advantages:

- High predictive performance
- Captures complex patterns


---

## 3. XGBoost Regressor

XGBoost was implemented for optimized gradient boosting.

Features:

- Regularization
- Faster training
- Better generalization


---

# ⚙️ Model Optimization

Performed hyperparameter tuning using:

```
GridSearchCV
```

Parameters optimized:

- Number of estimators
- Maximum depth
- Minimum samples split
- Feature selection


---

# 📈 Model Evaluation

Evaluation metrics:

## R² Score

Measures how well the model explains variance.

Higher value = better prediction.


## Mean Squared Error (MSE)

Measures average squared prediction error.


## RMSE

Measures prediction error magnitude.


## MAE

Measures average absolute error.

---

# 📉 Prediction Visualization

Generated:

- Actual vs Predicted plot
- Error analysis


Example:

```
Actual Capacity
        |
        |
        v

Predicted Capacity
```

---

# 🛠️ Technologies Used

## Programming

- Python


## Libraries

- Pandas
- NumPy
- Matplotlib
- Seaborn
- Scikit-learn
- XGBoost


## Environment

- Kaggle Notebook
- Jupyter Notebook


---

# 📁 Project Structure

```
Solar-Power-Plant-Prediction

│
├── solar-data.ipynb
│
├── README.md
│
└── dataset
    └── Solar_Power_Plant_Dataset.csv

```

---

# 🚀 How to Run

Clone repository:

```bash
git clone https://github.com/AJITHPS7/Solar-Power-Plant-Prediction.git
```

Install dependencies:

```bash
pip install pandas numpy matplotlib seaborn scikit-learn xgboost
```

Run notebook:

```bash
jupyter notebook
```

Open:

```
solar-data.ipynb
```

---

# 📌 Results

The project compares multiple regression algorithms:

| Model | Purpose |
|---|---|
| Random Forest | Baseline model |
| Gradient Boosting | Improved prediction |
| XGBoost | Advanced boosting model |

The final optimized model improves prediction performance through:

- Feature selection
- Data cleaning
- Hyperparameter tuning

---

# 🔮 Future Improvements

Future enhancements:

🔹 Deploy model using Flask/FastAPI

🔹 Create interactive dashboard using Streamlit

🔹 Add real-time solar monitoring data

🔹 Use deep learning models

🔹 Deploy using cloud services

---

# 👨‍💻 Author

**Ajith P S**

MCA Graduate | AI/ML | Data Engineering Enthusiast

GitHub:
https://github.com/AJITHPS7


⭐ If you find this project useful, consider giving it a star!
