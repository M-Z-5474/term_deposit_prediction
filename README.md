

```md
<h1 align="center">🎯 Term Deposit Subscription Prediction</h1>
<p align="center">Predicting if a client will subscribe to a bank's term deposit using ML and Explainable AI</p>

<p align="center">
  <img src="https://img.shields.io/badge/Project-Type%3A-Binary%20Classification-blue" />
  <img src="https://img.shields.io/badge/ML-Techniques%3A-LogReg%2C%20RF%2C%20XGB-green" />
  <img src="https://img.shields.io/badge/Explainable%20AI%3A-SHAP-yellow" />
</p>

---

## 📁 Dataset Overview

| Property           | Value                                    |
|--------------------|------------------------------------------|
| 📊 Source           | [UCI Bank Marketing Dataset](https://archive.ics.uci.edu/ml/datasets/bank+marketing) |
| 🧮 Total Records    | 41,189                                   |
| 🎯 Target Variable | `y` — subscription to term deposit (`Yes`/`No`) |

> 🔍 The dataset relates to direct marketing campaigns of a Portuguese banking institution.

---

## ✅ Project Objectives

- 🔢 Predict whether a client will subscribe to a term deposit.
- ⚙️ Preprocess and encode categorical data.
- 🤖 Train and evaluate classification models.
- 🧠 Use SHAP for local & global model explainability.
- 📊 Compare results and choose the best-performing model.

---

## 🔄 Project Workflow

### 1. 🧪 Data Exploration

- Checked data types and null values
- Visualized target distribution (class imbalance)
- Correlation analysis on numeric features

### 2. 🧼 Preprocessing

- Label encoded the target (`Yes` → 1, `No` → 0)
- One-hot encoded categorical features
- Standardized/Scaled numerical features

### 3. 🧠 Model Training

- **Logistic Regression**
- **Random Forest Classifier**
- **XGBoost Classifier**

### 4. 📊 Evaluation Metrics

- Accuracy, Precision, Recall, F1-Score
- Confusion Matrix
- ROC-AUC Curve

### 5. 🧠 Model Explainability

- Applied **SHAP** for:
  - Feature importance (global)
  - Explaining 5 individual predictions (local)

---

## 📊 Model Performance Summary

| Model         | Accuracy | Precision (1) | Recall (1) | F1-Score (1) | AUC  |
|---------------|----------|----------------|-------------|----------------|------|
| Logistic Reg. | 0.9007   | 0.70           | 0.21        | 0.32           | 0.80 |
| Random Forest | 0.8978   | 0.59           | **0.31**    | **0.40**       | 0.80 |
| XGBoost       | 0.8997   | 0.62           | 0.29        | 0.39           | 0.80 |

> ⚠️ Because of the class imbalance, **Recall and F1-Score for class "1"** are more important than accuracy.

---

## 🧾 Confusion Matrix (Class "1")

| Model         | TP  | FN  | FP  | TN   |
|---------------|-----|-----|-----|------|
| Logistic Reg. | 191 | 737 | 81  | 7229 |
| Random Forest | **286** | **642** | 200 | 7110 |
| XGBoost       | 266 | 662 | 164 | 7146 |

- ✅ **Random Forest** detects the most true positives and has the lowest false negatives.
- 🔍 Suitable for real use cases where "capturing Yes" is critical.

---

## 🧠 SHAP Explainability

| 🔍 Insights via SHAP |
|----------------------|
| 🔸 Top Features: `duration`, `poutcome`, `month`, `previous`, `campaign` |
| 🔸 SHAP summary plot shows global impact of features |
| 🔸 5 individual predictions explained with SHAP force plots |

📸 **Sample SHAP Summary Plot**  
<img src="shap_explanations.png" width="700"/>

---

## 🏁 Final Conclusion

🎉 **Random Forest Classifier** selected as the best-performing model:

- ✅ Highest recall and F1-score
- ✅ Most true positives
- ✅ Balanced precision vs. recall
- ✅ SHAP-compatible for explanations

---

## 🧠 Skills Highlighted

✅ Binary Classification  
✅ Data Preprocessing (Label/One-Hot Encoding)  
✅ Model Evaluation (with imbalanced classes)  
✅ Explainable AI (XAI)  
✅ Visualization & Reporting

---

## 🗂️ Project Structure

```

📁 Term-Deposit-Prediction/
│
├── 📄 term\_deposit\_prediction.ipynb     # Main Jupyter Notebook
├── 📄 shap\_explanations.png             # SHAP summary plot
├── 📄 README.md                         # This README file
└── 📁 data/                             # CSV dataset(s)

```

---

## 🚀 Deployment (Optional)

You could deploy the model using [Streamlit](https://streamlit.io/) to:

- 🧮 Let users input features (duration, month, etc.)
- 🔮 Predict if the client will subscribe
- 📊 Show SHAP explanation for each prediction

> 💡 This turns your notebook into a usable product.

---

## 📌 Tags

`Machine Learning` • `Binary Classification` • `Bank Marketing` • `Explainable AI` • `SHAP` • `Customer Prediction` • `Random Forest` • `XGBoost`

---

## 👤 Author

**Muhammad Zain Mushtaq**  
AI/ML & Data Science Enthusiast | Researcher  
📬 [LinkedIn](https://www.linkedin.com/in/muhammad-zain-m-a75163358/) • 📧 [mzainmushtaq@gmail.com](mailto:mzainmushtaq@gmail.com)

---

## 🌟 If you like this project, give it a ⭐ and share!
```

