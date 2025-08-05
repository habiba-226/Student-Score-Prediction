# Student Score Prediction

**Elovvo Machine Learning Internship – Level 1 Task**

## Task Overview

Build a regression model to predict students' **final exam scores** based on various performance-related features such as study hours, sleep, participation, and more.

This task covers the full ML pipeline including:
- Data cleaning
- Exploratory data analysis
- Model training and evaluation
- Result visualization

---

## Dataset

- **Source:** [Student Performance Factors – Kaggle](https://www.kaggle.com/datasets/lainguyn123/student-performance-factors) *(or similar dataset)*
- Contains features like:
  - Study hours
  - Sleep duration
  - Participation
  - Attendance
  - Distance from school
  - Teacher rating
  - Parental support
  - Internet access
  - ...and more

---

## 🛠️ Tools & Libraries

- Python
- Pandas
- Matplotlib / Seaborn
- Scikit-learn

---

## ✅ Project Workflow

### 1. Data Cleaning
- [x] Removed or imputed missing values
- [x] Encoded categorical features using one-hot encoding
- [x] Normalized numerical features if needed

### 2. Exploratory Data Analysis (EDA)
- [x] Visualized distributions and relationships
- [x] Checked feature correlation with final scores

### 3. Model Training
- [x] Split dataset into training (80%) and testing (20%)
- [x] Trained a Linear Regression model using `sklearn.linear_model.LinearRegression`

### 4. Evaluation Metrics
- [x] **Mean Squared Error (MSE):** `3.24`
- [x] **R² Score:** `0.771`

### 5. Visualization
- [x] Actual vs Predicted plot
- [x] Visualized feature importance (coefficients)

---

## 🎯 Results Summary

- The model shows good predictive power (R² ≈ 77%)
- Top influencing features were: study hours, participation, teacher rating, and sleep quality
- Coefficients revealed which factors positively or negatively affected performance

---

## 🚀 Bonus Ideas

- [ ] Apply **Polynomial Regression** and compare performance
- [ ] Try **Ridge / Lasso Regression** to reduce overfitting
- [ ] Feature selection to improve generalization
- [ ] Hyperparameter tuning for better accuracy

---

## 📌 Key Learnings

- Data preprocessing is essential for effective modeling
- Linear Regression is a great baseline model
- Understanding feature importance can guide education-related interventions

---

## Covered Concepts

- Regression modeling
- One-hot encoding
- Data splitting
- Evaluation metrics (MSE, R²)
- Feature analysis and interpretation
