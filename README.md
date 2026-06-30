# Customer Churn Prediction — Telecom Client Retention Strategy

**Author:** Febin Joseph  
**GitHub:** github.com/febinj86  
**Tools:** Python, Pandas, Scikit-learn, Matplotlib, Seaborn  

---

## Business Problem

A telecom company is experiencing significant customer churn, directly impacting revenue and long-term growth. This project analyses 7,043 customers to identify the key drivers of churn and build a predictive model to proactively retain at-risk customers.

---

## Dataset

- **Source:** Telco Customer Churn Dataset (Kaggle)
- **Size:** 7,043 customers, 21 features
- **Target Variable:** Churn (Yes/No)

---

## Methodology

1. Data Cleaning & Validation
2. Exploratory Data Analysis (EDA)
3. Feature Engineering
4. Model Building (Logistic Regression & Random Forest)
5. Model Evaluation

---

## Key Findings

- **26.5%** of customers are churning — 1 in 4 customers is leaving
- **Month-to-month** customers churn at 42.7% vs only 2.8% for two-year contracts
- **High-paying customers** (avg $80/month) churn significantly more than retained customers (avg $65/month)
- **New customers (0-10 months)** are the highest risk group — classified as the *Starting Section* in a custom three-tier segmentation framework:
  -  **Starting Section** (0-10 months) — highest churn risk
  -  **Decision Section** (10-20 months) — critical retention window
  -  **Stable Section** (20+ months) — low churn risk

---

## Model Results

| Model | Accuracy | Churners Correctly Identified |
|-------|----------|-------------------------------|
| Logistic Regression | 82% | 223 / 373 |
| Random Forest | 79.7% | 180 / 373 |

**Recommended Model:** Logistic Regression

---

## Business Recommendations

1. **Encourage longer contracts** — offer promotional discounts at contract renewal, especially for month-to-month customers
2. **Add value for high-paying customers** — bundle entertainment services (YouTube Premium, Spotify) to justify higher monthly charges
3. **Focus on new customer onboarding** — implement targeted retention plans for customers in the Starting Section (0-10 months)
4. **Deploy the model proactively** — use Logistic Regression predictions to identify and intervene with at-risk customers before they churn

---

## Technologies Used

- Python 3.10
- Pandas, NumPy
- Matplotlib, Seaborn
- Scikit-learn