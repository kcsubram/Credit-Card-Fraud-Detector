# Credit Card Fraud Detection

This project builds a full machine learning pipeline to detect fraudulent credit card transactions. It covers data exploration, preprocessing, imbalance handling, model training, and evaluation using several algorithms. The dataset used is the well-known Kaggle/ULB Credit Card Fraud Detection dataset, which is highly imbalanced and anonymized for privacy.


---

## 🎯 Project Objectives

- Understand and explore the credit card fraud dataset  
- Handle severe class imbalance  
- Build multiple fraud detection models  
- Compare performance using precision, recall, F1-score, and ROC-AUC  
- Produce a clean, reproducible ML workflow

---

## 🧠 Methods & Workflow

### **1. Data Understanding & Exploration**
- Loaded dataset and inspected structure  
- Checked for missing values  
- Explored distributions of:
  - `Amount`
  - `Time`
  - PCA-transformed features (`V1`–`V28`)
- Visualized class imbalance and transaction patterns  

---

### **2. Data Preprocessing**
- Scaled `Amount` and `Time`  
- Separated features and labels  
- Created train/test split  

---

### **3. Handling Class Imbalance**

Techniques explored:

- **Random Undersampling**
- **SMOTE (Synthetic Minority Oversampling Technique)**  

These methods help prevent model bias toward the majority (non-fraud) class.

---

### **4. Modeling**

You implemented and compared multiple ML models:

| Model | Notes |
|-------|-------|
| Logistic Regression | Baseline linear model |
| Random Forest | Strong performance, handles non-linear data |
| XGBoost | Highest performance for structured data |

---

### **5. Evaluation Metrics**

Evaluating fraud detection requires more than accuracy. Metrics used:

- **Precision**  
- **Recall**  
- **F1-score**  
- **Confusion matrix**  
- **ROC-AUC score**

High recall is essential because missing fraudulent transactions has high cost.

---

## 📊 Results (Summary)

While exact metrics differ per run, findings generally show:

- **Logistic Regression** → good baseline  
- **Random Forest** → strong and stable  
- **XGBoost** → best overall (highest ROC-AUC and recall)

---

## 🛠️ Installation & Setup

### **1. Install Dependencies**

pip install pandas numpy matplotlib seaborn scikit-learn imbalanced-learn xgboost lightgbm


### **2. Add Dataset**

Download the dataset from Kaggle:  
**"Credit Card Fraud Detection"**

Place `creditcard.csv` into a `data/` folder or update the notebook file path.

### **3. Run the Notebook**


---

## 📚 What This Project Demonstrates

- Real-world ML workflow  
- Handling extreme class imbalance  
- Comparing advanced ML algorithms  
- Proper evaluation of highly imbalanced data  
- Ability to structure a multi-week ML project

---

## 🚀 Future Improvements

- Hyperparameter tuning (GridSearchCV / Optuna)  
- Additional feature engineering  
- Model deployment (Flask/FastAPI)  
- Explainability using SHAP  

---

## ✨ Acknowledgments

Dataset:  
Kaggle – *Credit Card Fraud Detection Dataset*  
Originally published by ULB Machine Learning Group.

---

