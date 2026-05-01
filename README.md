Copy

🔄 Customer Churn Prediction — End-to-End Data Science Project
Show Image
Show Image
Show Image
Show Image

Final Data Science Project — Predicting customer churn in a telecom company using machine learning classification models.

📋 Table of Contents
Problem Statement
Dataset
Project Workflow
Tools & Technologies
Results
Folder Structure
How to Run
Key Visualizations
Business Recommendations
References
🎯 Problem Statement
Customer churn — when a customer stops using a service — is one of the most costly problems for telecom companies. Acquiring a new customer is 5–10x more expensive than retaining an existing one.

Goal: Build a machine learning model that predicts whether a customer will churn (Yes/No) based on account information, service usage, and demographic data — enabling the business to proactively target at-risk customers with retention strategies.

Success Metrics:

Accuracy > 80%
F1-Score > 0.75
ROC-AUC > 0.85
📦 Dataset
Property	Details
Name	Telco Customer Churn
Source	Kaggle — blastchar/telco-customer-churn
Rows	7,043 customers
Columns	21 features
Target	Churn (Yes / No)
Churn Rate	~26.5%
Key Features:

tenure — Months with the company
MonthlyCharges — Monthly billing amount
Contract — Contract type (Month-to-month / One year / Two year)
InternetService — DSL / Fiber optic / No
PaymentMethod — How the customer pays
SeniorCitizen — Whether customer is a senior
🔁 Project Workflow
Problem Definition
      ↓
Data Collection & Loading
      ↓
Data Cleaning & Preprocessing
      ↓
Exploratory Data Analysis (EDA)
      ↓
Feature Engineering
      ↓
Model Building (4 ML models)
      ↓
Model Evaluation (Accuracy, F1, AUC)
      ↓
Visualization of Results
      ↓
Conclusion & Business Recommendations
🛠️ Tools & Technologies
Category	Tools
Language	Python 3.10+
Data Manipulation	Pandas, NumPy
Visualization	Matplotlib, Seaborn
Machine Learning	Scikit-learn
Models Used	Logistic Regression, Decision Tree, Random Forest, Gradient Boosting
Notebook	Jupyter Notebook / Google Colab
Version Control	Git & GitHub
📊 Results
Model	Accuracy	F1-Score	ROC-AUC
Gradient Boosting	~84%	~79%	~88%
Random Forest	~83%	~77%	~87%
Logistic Regression	~80%	~74%	~85%
Decision Tree	~79%	~73%	~82%
✅ Best Model: Gradient Boosting

Top Predictive Features:

tenure — Customers with lower tenure churn more
MonthlyCharges — Higher charges increase churn risk
Contract — Month-to-month contracts have highest churn
TotalCharges — Reflects long-term relationship strength
InternetService — Fiber optic users churn more than DSL
📁 Folder Structure
customer-churn-prediction/
│
├── data/
│   ├── raw/
│   │   └── WA_Fn-UseC_-Telco-Customer-Churn.csv
│   └── processed/
│       └── churn_cleaned.csv
│
├── notebooks/
│   └── customer_churn_prediction.ipynb
│
├── src/
│   ├── data_cleaning.py
│   ├── feature_engineering.py
│   ├── train_model.py
│   └── evaluate_model.py
│
├── reports/
│   ├── figures/
│   │   ├── churn_distribution.png
│   │   ├── correlation_heatmap.png
│   │   ├── model_evaluation.png
│   │   ├── feature_importance.png
│   │   └── model_comparison.png
│   └── final_presentation.pdf
│
├── requirements.txt
├── README.md
└── LICENSE
🚀 How to Run
Option A — Local (Jupyter)
bash
# 1. Clone the repository
git clone https://github.com/YOUR_USERNAME/customer-churn-prediction.git
cd customer-churn-prediction

# 2. Install dependencies
pip install -r requirements.txt

# 3. Download dataset from Kaggle
# Place it in: data/raw/WA_Fn-UseC_-Telco-Customer-Churn.csv

# 4. Launch notebook
jupyter notebook notebooks/customer_churn_prediction.ipynb
Option B — Google Colab
Click the badge below to open in Colab:

Show Image

📈 Key Visualizations
Chart	Insight
Churn Distribution Pie	26.5% of customers churned
Churn by Contract Type	Month-to-month = highest churn rate
Tenure Distribution	New customers churn most
Monthly Charges Boxplot	Churned customers pay more
Correlation Heatmap	tenure & TotalCharges are strongly correlated
ROC Curves	Gradient Boosting best separates churn/no-churn
Feature Importance	tenure, MonthlyCharges, Contract are top predictors
💡 Business Recommendations
Offer loyalty plans to month-to-month customers in their first 3 months
Personalize retention campaigns for customers with high monthly charges
Bundle TechSupport & OnlineSecurity — these services reduce churn risk
Flag new customers (tenure < 6 months) for proactive outreach
Review Fiber Optic pricing — high charges drive dissatisfaction
🔮 Future Improvements
 Handle class imbalance using SMOTE
 Hyperparameter tuning with GridSearchCV / Optuna
 Add SHAP values for model explainability
 Deploy as REST API (Flask / FastAPI)
 Build interactive dashboard (Streamlit / Gradio)
 Experiment with XGBoost and LightGBM
📚 References
Azie88 — Customer Churn ML Classification (GitHub)
Kaggle Telco Customer Churn Dataset
Scikit-learn Documentation
Pandas Documentation
Seaborn Documentation
👤 Author
[Your Name]
Data Science Student
📧 youremail@example.com
🔗 GitHub Profile

📄 License
This project is licensed under the MIT License — free to use for educational and non-commercial purposes.

Submitted as Final Data Science Project — Week 8


