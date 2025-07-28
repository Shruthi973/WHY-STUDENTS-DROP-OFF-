# 🎓 Why Students Drop Off – Internship Churn Modeling

This data science project analyzes student churn in an AI-powered internship program with over **8,500 learners**. Using Python-based data pipelines, feature engineering, and classification models, we explore how behavioral and demographic signals relate to dropout.

<p align="center">
  <img src="STUDENT DROP-OFFS.jpg" width="600"/>
  <br>
  <em>⚙️ Predictive churn analysis to improve digital internship retention</em>
</p>

---

## 📁 Dataset

- **Size**: 8,529 student records
- **Target Variable**: `churned` (1 = Dropped, 0 = Retained)
- **Key Features**:
  - `application_lag_days` (delay in engagement)
  - `converted_binary`, `status_code`, `gender_encoded`, `age`, `active_weeks`
  - `country_code`, `language_code`, and derived features

---

## 🧠 Modeling Approach

We applied classification models using **Scikit-learn**, with imbalanced data handling and metric evaluation.

## 🤖 Models & Performance

| Model              | Accuracy | Precision | Recall | ROC AUC | Notes                                      |
|-------------------|----------|-----------|--------|---------|--------------------------------------------|
| **Logistic Regression** | 83.1%    | 77.8%     | 72.4%  | 0.812   | Strong baseline, interpretable coefficients |
| **XGBoost**             | 91.3%    | 85.7%     | 80.2%  | 0.864   | Best performer, captured non-linear effects |
| **Naive Bayes**         | 79.2%    | 75.1%     | 68.3%  | 0.793   | Fast but lower recall                       |

> 📌 **Top Predictor**: `application_lag_days` — students who delayed applying > 7 days were **2× more likely** to churn.

---


### 📈 Model Metrics (Best Model: Random Forest)
| Metric            | Value     |
|-------------------|-----------|
| Accuracy          | 92.3%     |
| Precision         | 84.6%     |
| Recall (Sensitivity) | 91.7% |
| F1 Score          | 88.0%     |
| ROC-AUC           | 0.936     |

> Note: Accuracy is high due to class imbalance; AUC, F1, and recall were prioritized.

---

## 🔍 Key Findings

- **Application delay** (`application_lag_days`) was the strongest churn predictor.
- Students aged 26+ showed slightly higher dropout risk.
- The model identified low-engagement and late-joiner patterns with high churn probability.

---

## 📂 Files in Repo

- `churnS_excelerate.ipynb`: Full modeling and analysis in Python
- `Churn Analysis Report.pdf`: Executive summary and visual insights
- `churn_table.html`: Interactive summary table with feature distributions

---

## 📌 Tools & Libraries

- Python, Pandas, NumPy, Matplotlib, Seaborn
- Scikit-learn (classification models)
- Imbalanced-learn (class weight tuning)
- Jupyter Notebook

---

## 📬 Contact

- 👩‍💻 Shruthi Reddy Vudem  
- 📧 vudemshruthireddy@gmail.com  
- 🔗 [LinkedIn](https://www.linkedin.com/in/shruthi-reddy-vudem1410)

---
> “Behind every dropout is a pattern — this project uncovers it through data.”
