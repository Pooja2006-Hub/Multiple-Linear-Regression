# 🏠 Boston Housing Price Prediction using Multiple Linear Regression

## 📌 Project Overview
This project focuses on predicting house prices in different neighborhoods using **Multiple Linear Regression**. The model analyzes various housing and environmental factors to estimate the median value of homes.

---

## 📂 Dataset
- Source: Kaggle  
- Link: https://www.kaggle.com/datasets/prateekmaj21/boston-housing-dataset  

### 📊 Features Used
- RM → Average number of rooms per dwelling  
- LSTAT → % lower status of the population  
- PTRATIO → Pupil-teacher ratio by town  
- INDUS → Proportion of non-retail business acres  
- NOX → Nitric oxide concentration  
- AGE → Proportion of old houses  

### 🎯 Target Variable
- MEDV → Median value of owner-occupied homes  

---

## ⚙️ Technologies Used
- Python 🐍  
- NumPy  
- Pandas  
- Matplotlib / Seaborn  
- Scikit-learn  

---

## 🚀 Steps Performed

### 1. Load Data
- Imported dataset using Pandas

### 2. Data Exploration
- Checked missing values  
- Used `df.describe()` for statistics  
- Visualized relationships using plots and correlation heatmap  

### 3. Data Preparation
- Selected relevant features:
  - RM, LSTAT, PTRATIO, INDUS, NOX, AGE  
- Target variable:
  - MEDV  
- Split dataset into training (80%) and testing (20%)  

### 4. Model Building
- Used **LinearRegression()** from sklearn  
- Trained model using training data  

### 5. Model Evaluation
- Predicted house prices  
- Calculated:
  - Mean Squared Error (MSE)  
  - R² Score  

### 6. Interpretation
- Analyzed model coefficients  
- Identified most influential features  
- Plotted actual vs predicted values  

---

## 🧠 Machine Learning Model
- **Algorithm:** Multiple Linear Regression  
- Predicts housing prices based on multiple independent variables  

---

## 📊 Evaluation Metrics
- **MSE (Mean Squared Error):** Measures prediction error  
- **R² Score:** Measures model accuracy (closer to 1 is better)  

---

## 📈 Visualization
- Scatter plot of Actual vs Predicted prices  
- Correlation heatmap for feature relationships  

---

## 🧾 Sample Code
```python
from sklearn.linear_model import LinearRegression

model = LinearRegression()
model.fit(X_train, y_train)

y_pred = model.predict(X_test)
