# Heart Attack Risk Prediction Model

## 📌 Project Overview

This project focuses on building a **machine learning–based Heart Attack Risk Prediction system** using clinical and lifestyle data. The goal is to identify individuals at **high risk of heart attack** as early as possible, with special emphasis on **high recall**, which is crucial in medical decision‑making.

The project covers the **complete ML pipeline** — data cleaning, exploratory data analysis (EDA), feature engineering, handling class imbalance, model training, and evaluation.



## 🎯 Objectives

* Analyze medical and lifestyle factors affecting heart attack risk
* Perform thorough **data cleaning and EDA** to uncover meaningful patterns
* Engineer medically relevant features
* Build a **robust and interpretable ML model**
* Prioritize **recall** to avoid missing high‑risk patients



## 📂 Repository Structure

```
├── Data (cleaned & uncleaned .csv files)
├── Heart_Attack_prediction (CTAI-013).ipynb   # Complete notebook (Data cleaning + EDA + Feature engineering + ML model)
└── README.md
```



## 📊 Dataset Description

* **Total Records:** 1,000 patients
* **Target Variable:** Heart Attack Risk (0 = Low, 1 = High)

### Key Features

**Medical Factors:**

* Age, Sex, Chest Pain Type
* Blood Pressure (Systolic & Diastolic)
* Cholesterol
* Heart Rate
* Diabetes, Fasting Blood Sugar
* ECG Results, ST Depression

**Lifestyle Factors:**

* Smoking, Obesity, Alcohol Consumption
* Exercise Hours per Week
* Physical Activity Days
* Stress Level
* Sleep Hours



## 📝Data Cleaning & EDA

* Removed duplicate and invalid records
* Handled missing values and outliers
* Standardized units and encodings
* Split combined BP column into systolic & diastolic
* Performed **univariate and bivariate analysis** using visualizations

### Key EDA Insights

* Higher **age, cholesterol, BP, BMI, stress** → higher risk
* Lower **exercise and sleep** → higher risk
* Diabetes and obesity strongly linked to heart attack risk



## ⚙️ Feature Engineering

* Created scaled medical indicators (BP, cholesterol, heart rate)
* Encoded categorical variables using label & one‑hot encoding
* Standardized continuous features
* Handled **class imbalance using SMOTEENN**

---

## Model Building

Multiple models were tested, and the **best-performing model was selected**:

### ✅ Final Model: XGBoost Classifier

**Why XGBoost?**

* Excellent performance on structured medical data
* Handles complex feature interactions
* Built‑in regularization to prevent overfitting
* Provides feature importance for interpretability
* Performs well on imbalanced datasets



## 📈 Evaluation Metrics

Medical‑focused evaluation was used:

* **Accuracy**
* **Precision**
* **Recall (Primary Focus)**
* **F1 Score**

> ⚠️ High recall ensures that high‑risk patients are not missed.

### Key Predictive Features

* Chest pain type
* Maximum heart rate achieved
* Resting blood pressure
* ST depression level
* Cholesterol

These align well with real‑world clinical knowledge.



## Conclusion

This project demonstrates how **data science and machine learning** can be applied to real healthcare problems. The final XGBoost model successfully identifies high‑risk individuals with strong recall, making it suitable as a **decision‑support tool** for early heart attack risk detection.



## 🚀 Future Improvements

* Improve Model Accuracy further
* Integrate SHAP for explainable AI
* Add more lifestyle & stress‑related features
* Deploy as a web or hospital decision‑support system
* Retrain model with newer patient data

