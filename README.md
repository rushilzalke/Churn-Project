📘 Customer Churn Prediction & Business Insights

An End-to-End Data Analytics + ML Project

📌 Project Summary

This project predicts telecom customer churn and converts the model outputs into actionable business insights, ROI analysis, and a professional dashboard.
It includes the full cycle: cleaning → feature engineering → model training → probability scoring → retention strategy → dashboard.

This project is designed to demonstrate data analytics skills, machine learning, business reasoning, and dashboard storytelling — perfect for Data Analyst/ML Analyst roles.

🗂 Project Structure
churn-project/
│
├─ data/
│  ├─ raw/                     # original dataset
│  └─ processed/               # cleaned datasets & train/test
│
├─ notebooks/
│  ├─ 01_data_exploration.ipynb
│  ├─ 02_feature_engineering.ipynb
│  ├─ 03_modeling_and_evaluation.ipynb
│  └─ 04_business_roi.ipynb
│
├─ artifacts/
│  ├─ best_pipeline.joblib     # saved model
│  ├─ preprocessor.joblib      # OHE + scaler
│  └─ high_risk_customers.csv  # predictions + probabilities
│
├─ reports/
│  ├─ roi_scenarios.csv        # scenario analysis output
│  ├─ dashboard_screenshots/   # dashboard images/GIF
│  └─ final_report.pdf         # optional
│
├─ powerbi/
│  ├─ churn_dashboard.pbix     # dashboard file (Power BI)
│  └─ streamlit_dashboard.py   # alternative Streamlit app
│
├─ models/
│  └─ saved models (optional)
│
├─ requirements.txt
└─ README.md

🧠 Objective

Identify customers most likely to churn

Understand why customers churn

Provide actionable retention strategies

Calculate revenue impact and ROI for interventions

Build a clean dashboard showcasing insights and high-risk customers

🧪 Tech Stack

Python: pandas, numpy, scikit-learn, matplotlib, seaborn, joblib

Machine Learning: Logistic Regression, Random Forest, XGBoost

Dashboarding: Power BI (primary), Streamlit (alternative)

Tools: Jupyter Notebooks, VS Code

🚀 1. Data Exploration & Cleaning

Notebook: 01_data_exploration.ipynb

Key Tasks

Loaded raw Telco Churn dataset

Handled missing values

Converted data types (e.g., TotalCharges → numeric)

Cleaned whitespace, standardized column names

Performed EDA:

Churn distribution

Monthly charges & tenure trends

Contract & payment method effects

Outputs

data/processed/churn_base.csv

Cleaned dataset ready for feature engineering

🛠 2. Feature Engineering

Notebook: 02_feature_engineering.ipynb

Features Added

Tenure buckets (0–12, 13–24, 25–48, 49+)

High-value customer flag

Service count / multiple services

Monthly average spend

OHE for categorical fields

Scaler for numerical features

Outputs

data/processed/churn_for_model.csv

preprocessor.joblib

🤖 3. Modeling & Evaluation

Notebook: 03_modeling_and_evaluation.ipynb

Models Trained

Logistic Regression

Random Forest

XGBoost

Evaluation Metrics

Accuracy

Precision, Recall, F1

ROC-AUC (main metric)

Confusion Matrix

Best Model

Random Forest (best AUC score)

Saved as best_pipeline.joblib

Outputs

Predictions with churn probability

high_risk_customers.csv (top risky customers)

💼 4. Business ROI Analysis

Notebook: 04_business_roi.ipynb

Computed:

ARPU (Average Revenue Per User)

Campaign cost assumptions

Retention success rate assumptions

3 ROI Scenarios:

Conservative

Realistic

Aggressive

Generated:

roi_scenarios.csv

Revenue saved

Expected retained customers

Net gain

ROI%

These numbers power the ROI dashboard page.

📊 5. Dashboard (Power BI & Streamlit)
✔ Power BI Dashboard

File: powerbi/churn_dashboard.pbix

4 Pages:

Page 1 — Overview

KPIs: Total Customers, Churn Rate, ARPU, High-risk Count

Donut: Churn distribution

Bar: Churn rate by tenure bucket

Insight commentary

Page 2 — Segmentation

Churn rate by contract

Churn by payment method

Spend distribution by churn

Slicers (Contract, Tenure bucket, Gender, Senior Citizen)

Page 3 — High-Risk Customers

Table with:

customer_id

churn_probability

predicted_churn

MonthlyCharges, Tenure, Contract

DAX-based Suggested Action

Conditional formatting (red → high risk, green → low risk)

Export enabled for business use

Page 4 — ROI & Business Impact

Scenario table

Revenue saved vs. campaign cost chart

Key metrics: Net Gain, ROI%

Action recommendations

✔ Streamlit Dashboard (Alternative)

File: powerbi/streamlit_dashboard.py

Run:

streamlit run powerbi/streamlit_dashboard.py


Provides:

KPIs

Churn segmentation

High-risk customer table

ROI scenarios

📈 Key Business Insights

Month-to-month contract customers churn 3× more than yearly contract customers.

Customers with low tenure (< 1 year) show the highest churn probability.

High monthly charges + no add-on services = high churn risk.

Targeting only the top 10–20% risky users yields the best ROI.

🗝 How to Run This Project
1. Clone the repo:
git clone <repo-url>
cd churn-project

2. Create environment:
pip install -r requirements.txt

3. Run notebooks:

Run in order:

01_data_exploration.ipynb

02_feature_engineering.ipynb

03_modeling_and_evaluation.ipynb

04_business_roi.ipynb

4. Run Streamlit dashboard (optional):
streamlit run powerbi/streamlit_dashboard.py

5. Open Power BI dashboard:

Open:

powerbi/churn_dashboard.pbix

🏆 Deliverables

Clean dataset

Feature-engineered dataset

ML model pipeline (joblib)

High-risk customer predictions

ROI scenario file

Full 4-page Power BI dashboard

Streamlit dashboard

Notebooks demonstrating full project workflow

✨ What This Project Demonstrates (For Recruiters)

Advanced data cleaning & feature engineering

Strong EDA storytelling

ML model building & tuning

Business problem framing

ROI-driven decision-making

Dashboard design & presentation

Production-like pipeline structuring

📬 Contact

Your Name
Email: replace@email.com

Role Target: Data Analyst / ML Analyst / Business Analyst