# 📓 Jupyter Notebook — Term Deposit Subscription Prediction

This folder contains the complete analysis, modeling, and explainability notebook for predicting whether a customer subscribes to a term deposit based on direct marketing efforts.

---

## 📄 File

- `term_deposit_prediction.ipynb`

---

## 🧠 Contents of the Notebook

1. **Exploratory Data Analysis (EDA)**
   - Overview of dataset shape, types, and imbalance
   - Correlation heatmaps and bar plots

2. **Preprocessing**
   - Label encoding for target variable
   - One-hot encoding for categorical columns
   - Feature scaling for numerical values

3. **Model Training**
   - Logistic Regression
   - Random Forest
   - XGBoost

4. **Evaluation**
   - Confusion matrix
   - Classification report (Precision, Recall, F1)
   - ROC-AUC scores and curves

5. **Explainability**
   - SHAP values for global and local explanation
   - Visual SHAP summary of top features
   - Individual prediction explanations for 5 samples

---

## 📌 How to Run

1. Make sure the `bank-full.csv` file exists in the `../dataset/` directory.
2. Open the notebook in Jupyter or Colab.
3. Run each cell in sequence to reproduce the analysis and model results.

---

## 💡 Highlights

- End-to-end binary classification project
- Proper handling of imbalanced data
- Interpretability using SHAP for transparency

