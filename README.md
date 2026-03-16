# Customer Churn Prediction

## 📌 Project Summary
This project predicts which customers are likely to leave a telecom company using the IBM Telco dataset. By training **Logistic Regression** and **Random Forest** models, it identifies key churn drivers such as month-to-month contracts, high monthly charges, and lack of tech support. Clear **visualizations and feature importance insights** guide proactive retention strategies. Results show that Random Forest performs best at catching high-risk customers, providing actionable business value.

---

## 🛠 Workflow & Key Steps

1. **Load and Inspect Data**
   - Loaded the IBM churn dataset (.csv)
   - Checked columns, data types, missing values

2. **Clean and Prepare Data**
   - Converted `Total Charges` to numeric, dropped invalid rows
   - Removed irrelevant columns: CustomerID, Churn Reason, CLTV, etc.

3. **Encode Categorical Variables**
   - Binary features (Yes/No, Male/Female) → LabelEncoder
   - Multi-category features (Contract, Payment Method, Services) → LabelEncoder

4. **Split Features and Target**
   - Target = Churn
   - Features = all other columns
   - Train/test split: 80% train, 20% test

5. **Train Models**
   - **Logistic Regression:** Accuracy ~0.81, F1-score for churn ~0.63
   - **Random Forest:** Higher accuracy and F1-score; better at predicting churn

6. **Analysis & Insights**
   - Feature importance shows top churn drivers
   - Month-to-month contracts, high charges, lack of tech support → higher churn probability
   - Visualized results with confusion matrices, heatmaps, and bar charts

---

## 🔧 Tools & Libraries
- Python  
- Pandas  
- NumPy  
- Scikit-learn  
- Matplotlib  
- Seaborn  

---

## 💼 Business Value
- Helps telecom companies identify and retain high-risk customers  
- Provides actionable insights for customer retention strategies  
- Supports data-driven decision-making  
