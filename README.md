# 🌧️ Rainfall Prediction Using Machine Learning

## 📌 Project Overview

Rainfall prediction is an important task in weather forecasting, agriculture, water resource management, and disaster prevention. This project uses Machine Learning techniques to predict whether rainfall will occur based on various meteorological parameters.

A Random Forest Classifier was trained on weather data and optimized using GridSearchCV to improve predictive performance. The project includes data preprocessing, exploratory data analysis, model training, hyperparameter tuning, evaluation, and prediction.

---

## 🎯 Objectives

- Analyze weather-related data.
- Predict the occurrence of rainfall.
- Compare model performance using multiple evaluation metrics.
- Optimize the model using hyperparameter tuning.
- Save the trained model for future predictions.

---

## 📂 Dataset

The dataset contains weather attributes that influence rainfall.

### Features

| Feature | Description |
|----------|-------------|
| pressure | Atmospheric pressure |
| dewpoint | Dew point temperature |
| humidity | Relative humidity |
| cloud | Cloud coverage |
| sunshine | Sunshine duration |
| winddirection | Wind direction |
| windspeed | Wind speed |

### Target Variable

| Variable | Description |
|-----------|------------|
| rainfall | Rainfall occurrence (Yes / No) |

Target encoding:
```python
yes → 1
no → 0
```

---

## 🛠️ Technologies Used

- Python
- NumPy
- Pandas
- Matplotlib
- Seaborn
- Scikit-Learn
- Pickle

---  

## 📊 Exploratory Data Analysis (EDA)

The following analyses were performed:

- Dataset inspection
- Missing value analysis
- Class distribution analysis
- Histograms
- Boxplots
- Correlation heatmap

### Visualizations

- Feature Distribution Plots
- Count Plots
- Boxplots
- Correlation Matrix Heatmap
- ROC Curve

---