# 📊 Regression Analysis on Pima Indians Diabetes Database
### Machine Learning Project – Regression Problem

---

## Table of Contents

1. [Project Overview](#project-overview)
2. [Dataset](#dataset)
3. [Data Preprocessing](#data-preprocessing)
4. [Exploratory Data Analysis (EDA)](#exploratory-data-analysis-eda)
5. [Modeling](#modeling)
6. [Evaluation](#evaluation)
7. [Results](#results)
8. [Presentation](#presentation)
9. [How to Run](#how-to-run)
10. [Acknowledgements](#acknowledgements)
11. [License](#license)
12. [توضیحات فارسی](#توضیحات-فارسی)

---

## Project Overview

[This project applies **regression models** to the [Pima Indians Diabetes Database](https://www.kaggle.com/datasets/uciml/pima-indians-diabetes-database) with the goal of predicting **blood glucose level** from various physiological and demographic features.  

The notebook walks through:
- Data loading and inspection  
- Handling missing values  
- Feature scaling and transformation  
- Applying and comparing multiple regression algorithms  
- Visualizing model performance

---

## Dataset

[- **Source:** Public dataset from [UCI Repository/Kaggle](https://www.kaggle.com/datasets/uciml/pima-indians-diabetes-database)  
- **Instances:** 768 rows (subset used in experiment)  
- **Features:** Pregnancies, Glucose, BloodPressure, SkinThickness, Insulin, BMI, DiabetesPedigreeFunction, Age, Outcome  
- **Target Variable:** `Glucose` (treated as continuous for regression)  
- **Missing Values:** Represented by `0` in certain features, replaced with median  

---

## Data Preprocessing

Steps implemented:
- Replace zeros in `BloodPressure`, `SkinThickness`, `Insulin`, `BMI` with `NaN`  
- Fill missing values using median imputation  
- Feature scaling using **StandardScaler**  
- Train/test split (80%/20%)

---

## Exploratory Data Analysis (EDA)

- Histograms for all features to observe distribution  
- Correlation matrix heatmap to assess feature relationships  
- Identified strongest correlations with the target variable `Glucose`  

---

## Modeling

The following regression models were implemented and compared:

1. **Linear Regression**  
2. **Ridge Regression**  
3. **Lasso Regression**  
4. **Polynomial Regression (degree=2)**  
5. **K-Nearest Neighbors Regression**  
6. **Support Vector Regression (RBF kernel)**  
7. **Decision Tree Regression**  
8. **Random Forest Regression**  
9. **Bayesian Ridge Regression**

---

## Evaluation

Metrics used:
- **Mean Squared Error (MSE)**
- **R² Score**

Also plotted:
- **Actual vs Predicted** values (scatter, all models plotted together)  
- **MSE & R² bar charts** for side-by-side comparison  

---

## Results

From the results in the notebook and presentation:
- Models like **Linear Regression, Ridge, Lasso, Polynomial, and Bayesian Ridge** achieved similar MSE (~500)  
- Decision Tree Regression showed high variance (overfitting tendencies)  
- R² score indicated moderate predictive capability – dataset may require more complex features or larger size for improvement

---

## Presentation

For visual summaries and Persian discussion of methodology & results, see:  
[`presentation.pdf`](presentation.pdf)

---

## How to Run

1. **Clone the repository:**
    ```bash
    git clone https://github.com/Arianafshar2003/Pima-Indians-Regression.git
    cd Pima-Indians-Regression
    ```
2. **Install dependencies:**
    ```bash
    pip install -r requirements.txt
    ```
3. **Open the notebook:**
    ```bash
    jupyter notebook code.ipynb
    ```
4. **Run cells sequentially** to reproduce preprocessing, modeling, and results.

---



## توضیحات فارسی

در این پروژه، دیتاست Pima Indians Diabetes برای پیش‌بینی سطح گلوکز خون با استفاده از مدل‌های رگرسیونی مورد استفاده قرار گرفته است. مراحل شامل:
1. بارگذاری و پاک‌سازی داده‌ها  
2. پیش‌پردازش و نرمال‌سازی  
3. اجرای چندین مدل رگرسیونی و مقایسه عملکرد  
4. ارزیابی مدل‌ها با شاخص‌های MSE و R²  


---

