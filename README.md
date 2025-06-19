# WHY-STUDENTS-DROP-OFF-
PYTHON AND R ANALYSIS 
## Student Churn Analysis – AI-Powered Internship Retention Study

This project explores churn behavior in an AI-powered virtual internship with 8,500+ learners. Through descriptive analytics and visual storytelling, it identifies churn predictors and offers strategic recommendations.

### 🔍 Project Highlights
- **Dataset**: 8,529 students | Application + Engagement + Demographics
- **Tools**: Python, Pandas, Seaborn, Matplotlib, Scikit-learn
- **Target Variable**: `churned` = 1 if student dropped out (Not Started / Applied)
- **Key Features**:
  - `application_lag_days`
  - `age`, `status_code`, `gender_encoded`
- **Modeling Attempted**: Classification models, but shifted to descriptive insights due to class imbalance (only ~1.2% churn rate)

### 📂 What's Inside
- `Churn Analysis Report.pdf`: Executive summary and visual report with churn predictors
- `churn_table.html`: Exploratory table with demographic + derived feature stats
- `churnS_excelerate.ipynb`: Full Python notebook with feature engineering, EDA, and modeling attempts

### 📊 Key Insight
Application delay was the strongest churn predictor—users who applied late were twice as likely to churn. Older students showed slightly higher dropout risk, potentially due to external constraints.
