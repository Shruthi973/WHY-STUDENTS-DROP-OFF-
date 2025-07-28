# 🎓 Why Students Drop Off – Internship Churn Modeling with Python

This project analyzes dropout patterns from a large AI internship program (~8,500 students) using machine learning and data science. It predicts student churn using real application, engagement, and demographic data — helping program managers intervene early.

<p align="center">
  <img src="STUDENT DROP-OFFS.jpg" width="600"/>
  <br>
  <em>🧠 AI-powered dropout detection using logistic modeling and XGBoost</em>
</p>

---

## 📁 Dataset Summary

- **Size**: 8,529 students  
- **Target**: `churned` = 1 if student dropped out before starting  
- **Key Features**:  
  - `application_lag_days`, `status_code`, `age`, `gender_encoded`, `state`  
  - Derived: `days_since_apply`, `enrollment_status`

---

## 🧪 ML Pipeline Overview

### 🔧 Preprocessing
- Null handling & encoding (`gender`, `state`)
- Derived features (application lag)
- Addressed class imbalance using **SMOTE** (churn rate ≈ 1.2%)

### 📊 EDA Highlights
- **Late applicants** showed ~2× churn risk  
- Slightly higher dropout among older learners  
- Engagement lag > 7 days strongly predicted churn

---

## 🤖 Modeling & Evaluation

### 1. **Logistic Regression**
- **Accuracy**: 83%
- **ROC AUC**: 0.81  
- ✅ Interpretable baseline — key predictors like `application_lag_days` had strong odds ratios

### 2. **XGBoost**
- **Accuracy**: 91%  
- **ROC AUC**: 0.86  
- ✅ Best performer; captured non-linear interactions  
- ⚠️ Slight overfitting observed without early stopping

### 3. **Naive Bayes**
- **Accuracy**: 79%  
- ✅ Fast and simple, but underfit due to feature independence assumption

---

## 📈 Metrics Explained
| Metric       | Meaning                                                       |
|--------------|---------------------------------------------------------------|
| **Accuracy** | % of correct predictions (works well if data is balanced)     |
| **ROC AUC**  | Model’s ability to distinguish churners vs. non-churners      |
| **Precision**| % of predicted churners who actually dropped                  |
| **Recall**   | % of actual churners correctly identified                     |

---

## 📂 Files Included

- `churnS_excelerate.ipynb`: Python ML notebook with preprocessing, modeling, and evaluation  
- `Churn Analysis Report.pdf`: Executive-level visual summary  
- `churn_table.html`: Feature exploration table  

---

## 🧰 Tech Stack
`Python`, `Pandas`, `Scikit-learn`, `XGBoost`, `SMOTE`, `Seaborn`, `Matplotlib`

---

## 🧠 Key Takeaway
> Students who delay engagement (especially > 5–7 days) show significantly higher churn risk. Targeted reminders and earlier onboarding could reduce dropout by ~30%.

---

## 📬 Contact
📧 vudemshruthireddy@gmail.com  
🔗 [LinkedIn](https://www.linkedin.com/in/shruthireddyvudem/)  
🌐 [Portfolio](https://shruthi973.github.io)
