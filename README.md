# Titanic Survival Prediction 🚢

## 📌 Project Overview
This project predicts whether a passenger survived the Titanic disaster using machine learning.  
It demonstrates a complete data science workflow including data cleaning, exploratory data analysis (EDA), feature engineering, model building, and evaluation.

---

## 🎯 Problem Statement
Given passenger details such as age, gender, class, and fare, predict whether the passenger survived the Titanic disaster.

This is a **binary classification problem**.

---

## 📊 Dataset
- Source: Titanic dataset
- Rows: 891
- Target Variable: `Survived` (0 = No, 1 = Yes)

---

## 🔍 Exploratory Data Analysis (EDA)
Key insights from EDA:
- Female passengers had a significantly higher survival rate.
- Passengers in higher classes (1st class) were more likely to survive.
- Age distribution was right-skewed.
- Missing values were present in Age, Cabin, and Embarked columns.

---

## 🧹 Data Cleaning
Steps performed:
- Filled missing `Age` values using median.
- Filled missing `Embarked` values using mode.
- Dropped `Cabin` column due to excessive missing values.
- Removed irrelevant text columns (`Name`, `Ticket`).

---

## 🛠 Feature Engineering
- Encoded `Sex` using binary encoding.
- Applied one-hot encoding to `Embarked` and `Pclass`.
- Prepared feature matrix and target variable.

---

## 🤖 Model Building
- Algorithm used: **Logistic Regression**
- Data split: 80% training, 20% testing
- `max_iter` set to 1000 to ensure convergence.

---

## 📈 Model Evaluation

### Confusion Matrix

[89 16]
[21 53]

## The model correctly identified 89 non-survivors and 53 survivors.

## It misclassified 16 non-survivors as survivors and missed 21 actual survivors.

## The model performs better at predicting non-survival than survival.


