# 📁 Dataset — Term Deposit Subscription

This folder contains the dataset used for the project **"Term Deposit Subscription Prediction — Bank Marketing Campaign"**.

---

## 📦 Dataset Source

- **Origin**: [UCI Machine Learning Repository - Bank Marketing Dataset](https://archive.ics.uci.edu/ml/datasets/bank+marketing)
- **File**: `bank-additional-full.csv`
- **Instances**: 41,189
- **Target Variable**: `y` (Binary — Yes/No)

---

## 🧾 Feature Summary

| Feature        | Description                                      |
|----------------|--------------------------------------------------|
| age            | Client's age                                     |
| job            | Job type (admin, technician, etc.)               |
| marital        | Marital status                                   |
| education      | Education level                                  |
| default        | Has credit in default?                           |
| balance        | Average yearly balance (euros)                   |
| housing        | Has housing loan?                                |
| loan           | Has personal loan?                               |
| contact        | Contact communication type                       |
| day            | Last contact day of the month                    |
| month          | Last contact month of year                       |
| duration       | Duration of last contact (in seconds)            |
| campaign       | Number of contacts performed during campaign     |
| pdays          | Days passed after last contact                   |
| previous       | Number of contacts before this campaign          |
| poutcome       | Outcome of previous campaign                     |
| y              | Term deposit subscription (target: yes/no)       |

---

## 🧹 Notes

- Null values are **not explicitly present**, but categorical features need proper encoding.
- The dataset is **imbalanced**, so special attention was given to Recall and F1-Score during model evaluation.

---

## 📁 Usage in Project

This dataset is used in the notebook:
> `notebook/term_deposit_prediction.ipynb`

