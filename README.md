# 🛒 Customer Purchase Prediction (ML Project)

## 📌 Project Overview
This project predicts whether a customer will make a purchase based on demographic and behavioral features.  
The dataset is sourced from Kaggle and contains **1,500 rows and 9 columns**.

The goal is to build machine learning models that classify **PurchaseStatus (0: No, 1: Yes)**.

---

## 📂 Dataset Features
- **Age**: Customer's age  
- **Gender**: 0 = Male, 1 = Female  
- **Annual Income**: Customer’s income in USD  
- **Number of Purchases**: Total purchases made  
- **Product Category**: 0 = Electronics, 1 = Clothing, 2 = Home Goods, 3 = Beauty, 4 = Sports  
- **Time Spent on Website**: In minutes  
- **Loyalty Program**: 0 = No, 1 = Yes  
- **Discounts Availed**: Number of discounts (0–5)  
- **PurchaseStatus (Target Variable)**: 0 = No, 1 = Yes  

---

## 🔎 Exploratory Data Analysis (EDA)
- Distribution plots for numeric & categorical features  
- Correlation heatmap  
- Scatter plots to analyze relationships  
- Insights:  
  - Loyalty program and website time are positively correlated with purchases  
  - Data is balanced (≈53% vs 47%)  

---

## ⚙️ Data Preprocessing
- Checked missing values → none  
- Removed 112 duplicates  
- One-hot encoded categorical features (ProductCategory)  
- Standardized numerical features  

---

## 🤖 Machine Learning Models
Trained and evaluated multiple classifiers:
- **Logistic Regression** → Test Accuracy: ~84%  
- **Support Vector Machine (SVM)** → Test Accuracy: ~86%  
- **Random Forest** → Test Accuracy: ~92% (with tuning)  
- **XGBoost** → Test Accuracy: ~92% (with tuning)  

### 📊 Example: XGBoost (after tuning)
| Metric   | Class 0 | Class 1 |
|----------|---------|---------|
| Precision| 0.92    | 0.93    |
| Recall   | 0.94    | 0.91    |
| F1-Score | 0.93    | 0.92    |

---

## 🚀 Results & Insights
- Best performing models: **Random Forest & XGBoost (≈92% accuracy)**  
- Logistic Regression gave interpretable but slightly weaker performance  
- Loyalty program, discounts availed, and website time were the strongest predictors  

