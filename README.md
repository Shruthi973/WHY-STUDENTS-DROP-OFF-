# 🎓 Why Students Drop Off – Data-Driven Churn Analysis in Virtual Internships

This project investigates **student churn behavior** in an AI-powered virtual internship platform with over 8,500 participants. It uses **EDA, feature engineering, and modeling** to uncover key dropout signals and inform targeted retention strategies.

<p align="center">
  <img src="STUDENT DROP-OFFS.jpg" width="600"/>
  <br>
  <em>⚡ Feature-driven churn analysis for education engagement</em>
</p>

---

## 📦 Dataset Summary

- **Observations**: 8,529 student records
- **Target**: `churned` (binary) – 1 if student did not complete onboarding
- **Features**:
  - `application_lag_days`: Days between opening and applying
  - `status_code`: Enrollment milestone
  - `age`, `gender_encoded`, and behavioral indicators
- **Challenge**: High class imbalance (~1.2% churn)

---

## ⚙️ Tools & Techniques

- **Languages**: Python (main), R (exploration)
- **Libraries**: `pandas`, `numpy`, `seaborn`, `matplotlib`, `scikit-learn`
- **Methods**:
  - Descriptive analytics with multi-variate breakdowns
  - Custom binning + ratio encodings for demographic insights
  - Class imbalance detection and early-stage modeling (LogReg, RF)
  - Feature scaling, visual correlation mapping

---

## 📊 Key Takeaways

- **Application lag** was the **strongest churn driver** — students who delayed applying were 2x more likely to drop out.
- **Age** showed minor correlation with churn (older learners = slightly higher attrition).
- **Modeling** was deprioritized due to extreme imbalance, shifting focus to high-impact EDA.

---

## 📂 Files

| File | Description |
|------|-------------|
| `churnS_excelerate.ipynb` | Full Python notebook with EDA, feature engineering, and model attempt |
| `Churn Analysis Report.pdf` | Executive summary + visuals for stakeholder presentation |
| `churn_table.html` | Tabular summary with feature-wise breakdown and group statistics |

---

## 🧠 Why It Matters

This study applies **practical ML workflows** to an imbalanced real-world problem — showing how **feature-driven EDA** can outperform brute-force modeling when the goal is **actionable insight**, not just prediction.

> Built for stakeholder clarity, technical soundness, and real-world usability in education analytics.

