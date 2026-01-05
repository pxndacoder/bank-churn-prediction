Retail Banking: Predictive Churn Pipeline & Risk Segmentation

📌 Project Overview

This project provides an end-to-end Machine Learning solution for a retail bank to identify customers likely to close their accounts. In competitive markets like Canada (RBC/CIBC) or the Caribbean (Sagicor), retaining high-value customers is 5x cheaper than acquiring new ones.

This pipeline doesn't just predict "who" leaves, but explains "why" they leave and quantifies the financial balance at risk.

🚀 Key Results

- Predictive Power: Achieved an 81% ROC-AUC using an optimized XGBoost model.

- Imbalance Handling: Utilized SMOTE to address the 7.7% minority churn class, ensuring high recall for at-risk customers.

- Business Impact: Identified $40M+ in deposits held by high-value "Platinum" customers currently in the critical risk tier.

🛠️ Data Science Workflow

1. Advanced Feature Engineering

Beyond raw data, I engineered 39 business-specific features:

- Service Friction Score: Tracks the correlation between unresolved complaints and fee burdens.

- Net Retention Score: A quantitative balance of "Anchors" (Mortgages, Direct Deposit) vs. "Risk Signals" (Inactivity, High Fees).

- Digital Adoption: Measuring mobile-first behavior as a predictor of loyalty.

2. Explainable AI (XAI)

Using SHAP, we moved beyond the "black box."

- Key Insight: Customers with only one product and no direct deposit are 4.2x more likely to churn.

- Visual Proof:

3. Model Performance

Comparison between baseline Logistic Regression and Gradient Boosting (XGBoost).

💼 Business Strategy & Dashboard

The model segments customers into a Risk-Value Matrix:

Segment Risk Tier Recommended Action
Platinum Critical Immediate RM Outreach & Fee Waivers
Gold High Targeted Lending Pre-approvals
Silver Medium Digital Engagement/Drip Campaign

Financial Exposure Dashboard

The pipeline generates interactive Plotly dashboards allowing executives to see exactly how much capital is at risk of leaving the bank.

📂 Repository Structure

- 1_data_generation.py: Creates synthetic banking dataset.

- 2_eda_and_cleaning.py: Automated cleaning and exploratory analysis.

- 3_feature_engineering.py: Transformation of raw data into banking insights.

- 4_modeling.py: Training, SMOTE, and Threshold Optimization.

- 5_explainability.py: SHAP analysis for feature contribution.

- 6_segmentation_dashboard.py: Risk-tiering and CRM-ready export.

⚙️ Setup & Installation

1. Clone the repo: git clone https://github.com/pxndacoder/bank-churn-prediction.git

2. Install requirements: pip install -r requirements.txt

3. Run the pipeline in order (1-6).

---

Author: pxndacoder

Industry focus: FinTech / Retail Banking Data Science
