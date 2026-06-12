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
- Histograms and Boxplots
- Correlation heatmap

### Visualizations
- Feature Distribution Plots
- Count Plots
- Boxplots
- Correlation Matrix Heatmap
- ROC Curve

---

## 🔧 Data Preprocessing

### Missing Value Handling
| Feature | Method Used |
|----------|-------------|
| winddirection | Mode Imputation |
| windspeed | Median Imputation |

### Feature Selection
Highly correlated temperature features were removed.

### Class Balancing
The dataset showed class imbalance.

To address this issue:
- Majority class was downsampled
- Minority class was retained
- Dataset was shuffled before training

---

## 🤖 Machine Learning Model

### Algorithm Used

```python
RandomForestClassifier
```

### Hyperparameter Tuning
GridSearchCV was used to optimize model performance.

---

## 📈 Model Evaluation

The model was evaluated using:

### Accuracy Score
Measures overall prediction performance.

### Precision
Measures the correctness of positive predictions.

### Recall
Measures the model's ability to identify rainfall events.

### F1 Score
Harmonic mean of Precision and Recall.

### Confusion Matrix
Displays:
- True Positives
- True Negatives
- False Positives
- False Negatives

### ROC-AUC Score
Measures the model's ability to distinguish between rainfall and non-rainfall events.

Interpretation:
```text
AUC = 0.5  → Random Guessing
AUC > 0.7  → Good Model
AUC > 0.8  → Very Good Model
```

### Cross Validation

5-Fold Cross Validation was used to evaluate model stability.

---

## 📉 ROC Curve

The ROC Curve compares the model's performance against a Random Baseline classifier.

- The diagonal dashed line represents random guessing.
- The closer the ROC curve is to the top-left corner, the better the model performs.
- A higher AUC score indicates stronger classification capability.

---

## 💾 Model Saving

The trained model is saved using Pickle.