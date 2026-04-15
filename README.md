# 🏦 Loan Approval Prediction System

## 📌 Overview

This project predicts whether a loan application will be approved or not using machine learning models. It includes data preprocessing, feature engineering, model training, and evaluation.

---

## 📊 Dataset

* Total records: 1000
* Features: 19 (before encoding)
* Target variable: `Loan_Approved`

### Key Features:

* Applicant Income, Coapplicant Income
* Credit Score
* Loan Amount & Term
* DTI Ratio, Savings, Collateral Value
* Employment, Education, Property Area

---

## ⚙️ Tech Stack

* Python
* Pandas, NumPy
* Seaborn, Matplotlib
* Scikit-learn

---

## 🔄 Workflow

### 1. Data Preprocessing

* Handled missing values using:

  * Mean (numerical)
  * Most frequent (categorical)
* Dropped irrelevant column: `Applicant_ID`

### 2. Encoding

* Label Encoding:

  * Education Level
  * Target Variable
* One-Hot Encoding:

  * Employment Status, Loan Purpose, etc.

### 3. Feature Scaling

* StandardScaler applied to normalize data

### 4. Feature Engineering

* Added:

  * `DTI_Ratio_sq`
  * `Credit_Score_sq`

---

## 🤖 Models Used

* Logistic Regression
* K-Nearest Neighbors (KNN)
* Naive Bayes

---

## 📈 Results (Before Feature Engineering)

| Model               | Accuracy |
| ------------------- | -------- |
| Logistic Regression | 86.5%    |
| Naive Bayes         | 86.5%    |
| KNN                 | 76%      |

---

## 🚀 Results (After Feature Engineering)

| Model               | Accuracy |
| ------------------- | -------- |
| Logistic Regression | ⭐ 88%    |
| Naive Bayes         | 86%      |
| KNN                 | 78.5%    |

---

## 🏆 Best Model

**Logistic Regression** achieved the highest accuracy after feature engineering.

---

## 📊 Key Insights

* Credit Score has strong positive impact on loan approval
* High DTI Ratio negatively affects approval
* Feature engineering improved model performance

---

## ▶️ How to Run

```bash
git clone <repo-link>
cd loan-prediction
pip install -r requirements.txt
python main.py
```

---

## 📌 Future Improvements

* Hyperparameter tuning
* Deploy as a web app (Streamlit/Flask)
* Use advanced models (XGBoost, Random Forest)

---

## 👤 Author

Gurbachan Singh
