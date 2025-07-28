# 🎓 Why Students Drop Off – Student Churn Prediction in Python

This project investigates student churn behavior in a large-scale AI internship program with over 8,500 records. Using Python, we built an end-to-end pipeline from data cleaning and feature engineering to exploratory analysis and classification modeling to detect dropout risk patterns.

<p align="center">
  <img src="STUDENT DROP-OFFS.jpg" width="600"/>
  <br>
  <em>📉 AI-powered insights into internship retention challenges</em>
</p>

---

## 📁 Dataset Overview

- **Size**: 8,529 student entries  
- **Target**: `churned` (1 = dropped out / no start)  
- **Features**:
  - `application_lag_days`, `status_code`, `age`, `gender_encoded`, `state`, `skill_interest`
  - Derived: `days_since_apply`, `enrollment_status`, categorical encodings

---

## 🧠 Machine Learning Pipeline

### 🔧 Preprocessing & Engineering
- Null imputation and categorical encoding
- Derived time-based churn flags
- SMOTE for class imbalance (1.2% churn)

### 📊 EDA & Visualization
- Seaborn, Pandas Profiling, and Matplotlib
- Demographic vs churn correlation
- Heatmaps for feature interaction

### 🤖 Modeling
- **Logistic Regression** – baseline and interpretable
- **XGBoost** – fine-tuned with grid search
- **Naive Bayes** – fast benchmarking
- Evaluated with Accuracy, ROC AUC, Precision-Recall Curve

---

## 📈 Key Insights
- **Application delay** was the strongest churn predictor.
- **Older students** showed slightly higher dropout risk.
- **Certain skill interests** (e.g., late-stage tech) were linked to higher churn probability.

---

## 📂 Files
- `churnS_excelerate.ipynb`: Full Python pipeline
- `Churn Analysis Report.pdf`: Executive visual summary
- `churn_table.html`: Feature summary & EDA table

---

## 🛠 Tools & Libraries
`Python`, `Pandas`, `Scikit-learn`, `XGBoost`, `Seaborn`, `Matplotlib`, `Imbalanced-learn (SMOTE)`

---

## 📬 Contact
📧 vudemshruthireddy@gmail.com  
🔗 [LinkedIn](https://www.linkedin.com/in/shruthireddyvudem/)  
🌐 [Portfolio](https://shruthi973.github.io)

---

> “A few days' delay in application can double your churn risk — timing matters in education analytics.”
