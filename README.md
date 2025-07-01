# LoyaltyLens-XGBoost-Powered-Churn-Detection-Engine

# 🔮 ChurnShield – Predicting & Preventing Customer Churn in E-Commerce

> A machine learning–powered solution to **detect at-risk customers**, generate actionable insights, and drive **retention-focused marketing** in the e-commerce space.

![ChurnShield Banner](https://img.shields.io/badge/Churn%20Prediction-XGBoost-blueviolet?style=for-the-badge)
![SMOTE](https://img.shields.io/badge/Class%20Imbalance-SMOTE-red?style=for-the-badge)
![License: MIT](https://img.shields.io/badge/License-MIT-green?style=for-the-badge)

---

## 🚀 Project Summary

**ChurnShield** is an end-to-end data science capstone project built to help e-commerce businesses answer a crucial question:

> _"Which customers are likely to stop buying—and what can we do to retain them?"_

By leveraging real customer data, machine learning (XGBoost), and SHAP explainability, we predict churn with **up to 97% accuracy** and generate targeted, profit-focused business recommendations.

---

## 📦 Dataset Overview

- **Size**: 3,941 customer records  
- **Target Variable**: `Churn` (0 = loyal, 1 = churn)  
- **Features**: 11 variables including customer behavior, complaints, distance, cashback, etc.  
- **Source**: Simulated e-commerce dataset (`E-commerce Customer Churn.csv`)

---

## 💡 Key Features Used

| Feature               | Description |
|------------------------|-------------|
| `Tenure`              | Months as customer |
| `Complain`            | Whether customer filed a complaint |
| `CashbackAmount`      | Total cashback received |
| `DaySinceLastOrder`   | Inactivity duration |
| `WarehouseToHome`     | Delivery distance |
| `SatisfactionScore`   | Self-reported satisfaction |
| `PreferedOrderCat`    | Most ordered category |
| *(+ other features)*  | ... |

---

## 🧠 ML Modeling Highlights

- ✅ Feature Engineering with Pipeline  
- ✅ Handling Class Imbalance using **SMOTE** & **Over Sampling** 
- ✅ Model selection with **XGBoost Classifier**  
- ✅ Performance tuning & 5-Fold Cross-Validation  
- ✅ Interpretability with **SHAP**  

---

## 📊 Model Performance

| Evaluation Type            | Accuracy | Precision (Churn) | Recall (Churn) | ROC AUC |
|----------------------------|----------|-------------------|----------------|---------|
| CV (60/20/20, no SMOTE)    | 93%      | 87%               | 71%            | 0.942   |
| Final Model (SMOTE + XGB) | **97%**  | **98%**           | **97%**        | **0.996** |

> 📌 **Result**: Final model can detect 96+ churners out of 100 with minimal false alarms.

---

## 📈 Business Impact

🔎 Based on SHAP explainability, the top drivers of churn include:
- Short customer lifetime (low `Tenure`)  
- Recent complaints (`Complain = 1`)  
- Low cashback incentives  
- High delivery distance  

---

## 💬 Actionable Business Recommendations

| Segment                  | Recommendation                          | Expected Impact |
|--------------------------|------------------------------------------|-----------------|
| New users (Tenure < 3 mo)| Welcome campaign, onboarding cashback    | ⬆️ Retention    |
| Complainers              | Auto follow-up + apology voucher         | ⬇️ Churn        |
| Inactive users           | Re-engagement promo after 30 days        | ⬆️ Repeat order |

---

> 💡 Retaining 96 churners per month at 1.5M value = significant recurring impact.

---

## 📂 Project Structure

