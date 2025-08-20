
# Financial Risk Analysis & Prediction 📊

![Python](https://img.shields.io/badge/python-3.8%2B-blue.svg)
![License: MIT](https://img.shields.io/badge/License-MIT-green.svg)
![Machine Learning](https://img.shields.io/badge/Machine%20Learning-LogReg%20%7C%20RandomForest-orange)
![Contributions](https://img.shields.io/badge/contributions-welcome-brightgreen.svg)

This repository presents a **Financial Risk Analysis (FRA)** project that applies **machine learning techniques** to assess the financial health of companies and predict defaults.  
Additionally, it includes a **stock price analysis** of selected companies to provide investment insights.  

---

## 📂 Project Structure

### Part A – Company Default Prediction (Logistic Regression)
- Data preprocessing (missing values, zero handling, outlier treatment, scaling).
- Feature selection using VIF and Recursive Feature Elimination (RFE).
- Model building with Logistic Regression.
- **Final Model Performance**:  
  - Recall: **95%**  
  - Precision: **78%**  
  - Accuracy: **96%**  
  - F1 Score: **86%**  
- Focus: Identify companies at risk of **financial default**.

### Part B – Advanced Modeling & Stock Analysis
- Comparison of **Logistic Regression, LDA, and Random Forest**.
- Random Forest achieved the best performance:  
  - Accuracy: **96%**  
  - Precision: **93%**  
  - Recall: **76%**  
  - F1 Score: **0.84**  
- **Stock Price Analysis** of Infosys, Sun Pharma, Axis Bank, Shree Cement, etc.  
- Recommendation: **Infosys** and **Shree Cement** as strong investment options due to higher returns with lower volatility.

---

## 🗂 Dataset

- **Source:** Financial statements of 4256 companies (2015 data).  
- **Target Variable:** Net worth in the following year (2016).  
  - Default = 1 → Negative net worth.  
  - Default = 0 → Stable or positive net worth.  
- **Features:** 50+ financial ratios & balance sheet metrics.  

---

## ⚙️ Preprocessing Steps

1. Missing Value Treatment (KNN Imputer).  
2. Zero Value Handling (drop >30% zero columns, impute others).  
3. Outlier Treatment (IQR and Z-Score methods).  
4. Feature Scaling (Z-Score standardization).  
5. Multi-Collinearity Removal (VIF > 5).  
6. Feature Selection via Recursive Feature Elimination (RFE).  

---

## 🛠️ Technologies Used

- **Python**  
- Libraries:  
  `pandas`, `numpy`, `matplotlib`, `seaborn`,  
  `scikit-learn`, `statsmodels`, `imblearn` (SMOTE).  
- Jupyter Notebook for experimentation.  

---

## 📊 Results

- Logistic Regression Model #8 chosen as **final model** for company default prediction.  
- Random Forest performed best in **Part B** due to robustness and ease of hyperparameter tuning.  
- Stock Analysis shows **Infosys & Shree Cement** as reliable investment opportunities.  

---

## 🚀 How to Run

1. Clone this repository:
   ```bash
   git clone https://github.com/<your-username>/financial-risk-analysis.git
   cd financial-risk-analysis
