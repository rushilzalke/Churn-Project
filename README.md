[![Python](https://img.shields.io/badge/Python-3.10%2B-blue?logo=python)]()  
[![Power BI](https://img.shields.io/badge/PowerBI-Dashboard-F2C811?logo=powerbi&logoColor=white)]()  
[![Machine Learning](https://img.shields.io/badge/Machine%20Learning-Sklearn-orange)]()  
[![Status](https://img.shields.io/badge/Project-Complete-brightgreen)]()  
[![License](https://img.shields.io/badge/License-MIT-green)]()

---

## 🚀 Overview  
This project is a complete **end-to-end Customer Churn Analysis & Prediction system** built using:

- **Python** for data cleaning, EDA, feature engineering, ML  
- **Scikit-learn** pipelines for model building  
- **Power BI** for business dashboards  
- **Interpretability & ROI analysis** for actionable business insights  

🔍 Goal:  
Identify customers likely to churn & provide data-backed business actions to reduce churn.

---

## 📥 **Dataset**
The dataset used is the **Telco Customer Churn** dataset containing customer demographics, services used, contract type, billing info, and churn status.

---

## 🧹 **1. Data Cleaning & Preprocessing**  
Performed in `01_data_exploration.ipynb`:

- Handled missing values  
- Converted `TotalCharges` into numeric  
- Removed duplicates  
- Cleaned column types  
- Removed inconsistent entries  

Processed datasets saved under:

data/processed/
├── churn_cleaned.csv
├── churn_train.csv
└── churn_test.csv

yaml
Copy code

---

## 📊 **2. Exploratory Data Analysis (EDA)**  
Performed in `01_data_exploration.ipynb`:

✔ Churn distribution  
✔ Churn by contract  
✔ Churn vs Tenure  
✔ Churn vs Payment method  
✔ Correlation analysis  
✔ Revenue & charges distributions  

📸 **Dashboard image placeholder**

> Replace with your screenshot  
> File path example: `reports/dashboard_screenshots/eda.png`

```markdown
![EDA](reports/dashboard_screenshots/eda.png)
🧠 3. Feature Engineering
Performed in 02_feature_engineering.ipynb:

Engineered new features:

Tenure buckets

Average monthly spend

Number of subscribed services

High-value customer flags

Binary contract flags

Payment method indicators

These improved model performance significantly.

🤖 4. Machine Learning Modeling
Performed in 03_modeling_and_evaluation.ipynb:

Models Built:

Logistic Regression (baseline)

Random Forest (tree-based)

XGBoost (best performer)

Metrics Evaluated:

Accuracy

Precision

Recall

F1-score

ROC-AUC

📈 Random Forest delivered the best overall balance of Recall & AUC, ideal for churn prevention.

Saved model artifacts (joblib) located in:

Copy code
artifacts/
 ├── rf_pipeline.joblib
 ├── logistic_pipeline.joblib
 └── high_risk_customers.csv
💼 5. Business ROI Analysis
Performed in 04_business_roi.ipynb:

Calculated:

Avg Revenue per User (ARPU)

Revenue loss from churn

Cost of retention campaign

Expected savings from churn reduction

CSV export available:

bash
Copy code
reports/roi_scenarios.csv
📊 6. Power BI Interactive Dashboard
🔗 Download Dashboard (.pbix)
👉 Click here to download New.pbix

Dashboard includes:

Overall churn metrics

Churn segmentation (tenure, contract, services)

Revenue at risk

High-risk customer list (from ML model)

Suggested retention actions

📸 Dashboard preview placeholder
Replace with your screenshot:

markdown
Copy code
![Dashboard](reports/dashboard_screenshots/dashboard_page.png)
🗂️ Project Structure
css
Copy code
Churn-Project/
│
├── data/
│   ├── raw/
│   └── processed/
│
├── notebooks/
│   ├── 01_data_exploration.ipynb
│   ├── 02_feature_engineering.ipynb
│   ├── 03_modeling_and_evaluation.ipynb
│   └── 04_business_roi.ipynb
│
├── artifacts/
│   ├── high_risk_customers.csv
│   └── preprocessor.joblib
│
├── powerbi/
│   └── New.pbix
│
├── reports/
│   └── roi_scenarios.csv
│
├── src/
│   ├── data_prep.py
│   ├── feature_engineering.py
│   ├── model.py
│   └── utils.py
│
├── requirements.txt
└── README.md
⚙️ Installation
bash
Copy code
pip install -r requirements.txt
Run notebooks using Jupyter or VS Code.

🟢 Tech Stack
Python (Pandas, NumPy, Seaborn, Matplotlib)

Scikit-learn

Joblib

Power BI

Jupyter Notebook

Git / GitHub

📌 Key Insights
Month-to-month customers have highest churn

Electronic check customers churn more

Tenure < 12 months shows max churn risk

Senior citizens have slightly higher churn

Auto-pay + long-term contracts reduce churn drastically

🧠 Impact
💰 Up to 22% churn reduction possible using ML-driven targeting
📈 Retention campaigns show positive ROI
🎯 High-risk customers list helps allocate marketing budget efficiently

📄 License
MIT License.

🙌 Author
Rushil Zalke
Feel free to connect or explore my GitHub for more projects.
