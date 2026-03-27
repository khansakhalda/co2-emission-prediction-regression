# 🚗 CO2 Emission Prediction using Machine Learning

This project focuses on predicting **CO2 emissions from vehicles** using 
**machine learning regression techniques** and analyzing the impact of 
various vehicle attributes on emission levels.

Understanding emission patterns is important for environmental sustainability 
and data-driven policy making in the automotive industry.

---

## 📌 Background

Vehicle emissions are one of the main contributors to air pollution and climate change. 
Understanding the factors that influence CO2 emissions is crucial for developing 
effective environmental strategies.

However, emission levels are influenced by multiple variables such as engine size, 
fuel consumption, and vehicle characteristics, making it difficult to analyze manually.

This project uses machine learning regression to uncover relationships between 
vehicle features and CO2 emissions, and to build predictive models with high accuracy.

---

## 🎯 Objectives

This project aims to:

- Predict **CO2 emissions** based on vehicle attributes  
- Analyze which variables have the strongest impact on emissions  
- Compare multiple regression models using different feature combinations  
- Evaluate model performance using multiple metrics  
- Provide insights for environmental and automotive analysis  

---

## ⚙️ Process

### 1. Data Collection
- Dataset: Vehicle fuel consumption and CO2 emissions  
- Target variable: **CO2EMISSIONS**

---

### 2. Data Preprocessing
- Handling numerical and categorical variables  
- Encoding categorical features using **One-Hot Encoding**  
- Scaling numerical features using **StandardScaler**

---

### 3. Feature Engineering & Modeling

Tested multiple regression models using different feature combinations:

#### 🔹 Numerical Models
- ENGINESIZE  
- CYLINDERS + ENGINESIZE  
- FUELCONSUMPTION_CITY + ENGINESIZE  
- FUELCONSUMPTION_COMB + ENGINESIZE  
- FUELCONSUMPTION_COMB_MPG + ENGINESIZE  

#### 🔹 Categorical Models
- MAKE + ENGINESIZE  
- MODEL + ENGINESIZE  
- VEHICLECLASS + ENGINESIZE  
- TRANSMISSION + ENGINESIZE  
- FUELTYPE + ENGINESIZE  

#### 🔹 Full Model
- Combination of all features

---

### 4. Model Training
- Algorithm: **Ridge Regression**
- Train-test split: **80% training / 20% testing**

---

### 5. Model Evaluation

Evaluation metrics used:
- MAE (Mean Absolute Error)  
- RMSE (Root Mean Squared Error)  
- MSE (Mean Squared Error)  
- MAPE  
- R-squared  

---

## 📊 Results

### 🔹 Best Individual Model
- Features: **FUELCONSUMPTION_COMB_MPG + ENGINESIZE**
- R²: **0.887**
- MAE: **14.283**
- RMSE: **21.583**

---

### 🔹 Best Overall Model (All Features)
- MAE: **3.729**
- RMSE: **6.048**
- MAPE: **1.595%**
- R²: **0.991**

👉 Indicates extremely high prediction accuracy

---

## 💡 Key Insights

- **Fuel consumption is the strongest predictor of CO2 emissions**
- Engine size and number of cylinders strongly influence emissions
- Higher fuel consumption → higher emissions (strong positive correlation)
- MPG (fuel efficiency) has a **negative correlation** with CO2 emissions  
  → more efficient vehicles produce less emissions

- Using multiple features significantly improves model performance:
  - Single feature model → R² ≈ 0.76  
  - Multi-feature model → R² ≈ 0.99  

👉 This shows that CO2 emissions are influenced by **multiple interacting factors**, not just one variable.

---

## 🌍 Business / Real-World Insight

- Helps automotive companies design **more fuel-efficient vehicles**
- Supports government policy in reducing emissions
- Can be used for:
  - Emission prediction systems  
  - Environmental impact analysis  
  - Sustainable transportation planning  

---

## 🛠️ Technologies Used

- Python  
- Pandas, NumPy  
- Matplotlib, Seaborn  
- Scikit-learn  

---

## 👩‍💻 Author

Khansa Khalda  
Machine Learning Project  
Jenderal Soedirman University
