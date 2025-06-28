# 💳 Credit Risk Classifier using Decision Tree

A machine learning project to predict whether a loan applicant is a **good** or **bad credit risk** using the [kaggle German Credit Dataset with Target](https://www.kaggle.com/datasets/kabure/german-credit-data-with-risk/suggestions).

---

## 📊 Project Objective
To build and evaluate a classification model that predicts the creditworthiness of applicants based on demographic and financial features.

---

## 🧠 Algorithms Used
- ✅ Decision Tree Classifier (with pre-pruning)
- ✅ GridSearchCV for hyperparameter tuning

---

## 📂 Dataset Overview
- Source: UCI Machine Learning Repository  
- Samples: 1000  
- Features: `Age`, `Job`, `Housing`, `Saving accounts`, `Checking account`, `Credit amount`, `Duration`, `Purpose`, etc.  
- Target: `Risk` (good/bad)

---

## 🔧 Key Steps Performed

### 📌 Data Preprocessing
- Handled missing values using mode imputation for categorical fields
- Applied One-Hot Encoding for multi-class categorical features
- Scaled numerical features (`Age`, `Credit amount`, `Duration`) using **RobustScaler**

### 🧪 Model Training
- Trained a **Decision Tree Classifier** with:
  - Pre-pruning (`max_depth`, `min_samples_split`, `min_samples_leaf`)
  - `class_weight='balanced'` to handle class imbalance

### 📈 Evaluation
- Confusion Matrix
- Precision, Recall, F1-Score
- **ROC Curve** and **AUC Score**
- Comparative ROC plots between multiple decision tree configurations

---

