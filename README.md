### Bank Marketing Campaign – EDA & ML Model Exploration

📌 **Project Overview**
- This project analyses a bank marketing dataset from a Portuguese financial institution. The goal is to predict whether a customer will subscribe to a term deposit based on past interactions and demographic/economic factors.
- By combining EDA and machine learning models, this project provides insights into customer behaviour and helps improve marketing campaign efficiency.

📂 **Dataset**
- Source: UCI Bank Marketing Dataset (bank-additional.csv)
- Target variable: y (yes/no – whether the client subscribed to a term deposit)
- Features: demographic details, contact type, campaign history, and macroeconomic indicators

🔍 **Exploratory Data Analysis (EDA)**
_Key findings from EDA:_
- **Job type:** Students & retired people had the highest conversion rates.
- **Education:** Illiterates & unknown categories converted most, followed by university grads.
- **Marital status:** Married clients were more likely to subscribe.
- **Contact style:** Mobile phone contacts were far more effective than landline calls.
- **Seasonality:** May–August saw the highest conversion rates.
- **Day of week:** Conversions were fairly stable; Thursday performed slightly better.
- **Correlations:** Call duration and employment/economic indicators were the strongest predictors.

🤖 _**Models Implemented**_
1. **Logistic Regression** – Baseline linear model
2. **Decision Tree** – Simple interpretable tree model
3. **Random Forest** – Ensemble of trees, improved reliability
4. **XGBoost** – Boosting algorithm, best performing

📊 _**Results & Insights**_
- _Logistic Regression:_ Good accuracy (86%) but struggled with subscriber precision.
- _Decision Tree:_ Interpretable but unstable.
- _Random Forest:_ Explained ~41.5% variance; relied heavily on call duration.
- _XGBoost:_ Best trade-off between accuracy and generalisation.

**Key Drivers Identified:**
1. Employment indicators
2. Call duration
3. Previous campaign success
4. Economic conditions (e.g., euribor3m, nr.employed)

🚀 **Final Takeaways**
- **Best Model:** _**XGBoost**_
- _Actionable Insights for the Bank:_
  1. Prioritize high-potential customers for outreach
  2. Optimize call duration & timing to improve conversions
  3. Align campaigns with favorable economic conditions

✅ _**Impact:**_ _More efficient campaigns → reduced costs → higher conversion rates_

🛠️ **Tech Stack**
- Python (Pandas, NumPy, Scikit-learn, XGBoost)
- Jupyter Notebook
- Matplotlib / Seaborn for visualization
