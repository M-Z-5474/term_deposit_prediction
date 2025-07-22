
# 🎯 Term Deposit Subscription Prediction — Bank Marketing Campaign

![bank-marketing](https://img.shields.io/badge/Project-Type%3A-Binary%20Classification-blue)
Predict whether a customer will subscribe to a **term deposit** based on a direct marketing campaign using ML techniques and explainable AI.

---

## 📁 Dataset

* **Source**: [UCI Machine Learning Repository - Bank Marketing Dataset](https://archive.ics.uci.edu/ml/datasets/bank+marketing)
* **Records**: 41,189
* **Target Variable**: `y` (Yes/No — term deposit subscription)

---

## 📌 Objectives

✅ Predict whether a bank client will subscribe to a term deposit
✅ Encode and preprocess the dataset properly
✅ Train and evaluate classification models
✅ Use Explainable AI (SHAP) for interpreting predictions
✅ Compare model performance and choose the best

---

## 🛠️ Workflow

### 1. 📊 Data Exploration

* Checked for null values and data types
* Visualized class imbalance
* Explored correlations

### 2. 🧹 Preprocessing

* Label encoded the target variable
* One-hot encoded categorical features
* Scaled numerical values (where needed)

### 3. 🧠 Models Trained

* Logistic Regression
* Random Forest Classifier
* XGBoost Classifier

### 4. 📈 Evaluation Metrics

* Confusion Matrix
* Precision, Recall, F1-Score
* ROC-AUC Curve

### 5. 🧠 Explainability

* Used **SHAP** to explain **5 individual predictions** from the best model
* Plotted SHAP summary for global feature importance

---

## 📊 Model Performance Summary

| Model         | Accuracy | Precision (1) | Recall (1) | F1-Score (1) | AUC  |
| ------------- | -------- | ------------- | ---------- | ------------ | ---- |
| Logistic Reg. | 0.9007   | 0.70          | 0.21       | 0.32         | 0.80 |
| Random Forest | 0.8978   | 0.59          | **0.31**   | **0.40**     | 0.80 |
| XGBoost       | 0.8997   | 0.62          | 0.29       | 0.39         | 0.80 |

> 🔎 **Accuracy ≈ 90%** across all models, but since the dataset is imbalanced, **F1-Score and Recall for class 1 (Yes)** are more meaningful.

---

## ✅ Confusion Matrix (for Class `1` - Subscription)

| Model         | TP (1)  | FN  | FP  | TN   |
| ------------- | ------- | --- | --- | ---- |
| Logistic Reg. | 191     | 737 | 81  | 7229 |
| Random Forest | **286** | 642 | 200 | 7110 |
| XGBoost       | 266     | 662 | 164 | 7146 |

* 🔸 **Random Forest** catches **most true positives** (286), making it better for capturing actual subscribers.
* 🔸 It also has the **lowest false negatives**, reducing missed "Yes" predictions.

---

## 🧠 Model Interpretability with SHAP

Used SHAP (SHapley Additive exPlanations) to:

* Visualize **feature importance**
* Explain **5 individual predictions** with local interpretation plots
* Identify key factors influencing "Yes" and "No" predictions

> 💡 Top impactful features: `duration`, `month`, `poutcome`, `previous`, `campaign`

---

## 🏁 Final Verdict

> ✅ **Random Forest** is the **best overall model** based on:
>
> * Highest **Recall** and **F1-score** for minority class (1)
> * Most **True Positives** in Confusion Matrix
> * Balanced trade-off between precision and recall
> * Reliable performance and interpretability using SHAP

---

## 📚 Skills Demonstrated

* ✅ Data preprocessing & encoding
* ✅ Binary classification modeling
* ✅ Model evaluation with imbalanced data
* ✅ Explainable AI (XAI) with SHAP
* ✅ Customer behavior analytics

---

## 📎 Repository Structure

```
📁 Term-Deposit-Prediction/
│
└── 📁 notebook/   
     ├── 📄 term_deposit_prediction.ipynb     # Complete notebook with all steps
     └── 📄README.md                          # notebook readme file
├── 📁 dataset/                         
     ├── 📄 bank-additional-full.csv             # Dataset file
     └── 📄 README.md                          # Dataset README file
└──  📄 README.md                         # This file

```



## 🚀 Project Highlights

* ✅ 3 models trained, evaluated, and compared
* ✅ SHAP-based interpretability used
* ✅ Real-world imbalanced classification problem tackled

---

## 🤝 Contact

**Muhammad Zain Mushtaq**
AI/ML & Data Science Enthusiast | Researcher
📬 [LinkedIn](https://www.linkedin.com/in/muhammad-zain-m-a75163358/) | 📧 [mzainmushtaq@gmail.com](mailto:mzainmushtaq@gmail.com)

---

## 🌟 If you like this project, give it a ⭐ and share!
