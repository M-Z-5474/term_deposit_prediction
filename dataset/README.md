
# 📁 Dataset — Term Deposit Subscription

This folder contains the dataset used for the project:

> **🎯 Term Deposit Subscription Prediction — Bank Marketing Campaign**

---

## 📦 Dataset Source

* **🔗 Origin**: [UCI Machine Learning Repository - Bank Marketing Dataset](https://archive.ics.uci.edu/ml/datasets/bank+marketing)
* **📄 File**: `bank-additional-full.csv`
* **🔢 Instances**: `41,188 rows 
* **🎯 Target Variable**: `y` — Whether the client subscribed to a term deposit (Binary: `yes` or `no`)

---

## 🧠 Feature Overview

| 🧾 Column Name   | 📘 Description                                      | 🧮 Type  |
| ---------------- | --------------------------------------------------- | -------- |
| `age`            | Client's age                                        | `int`    |
| `job`            | Type of job (admin., technician, blue-collar, etc.) | `object` |
| `marital`        | Marital status (single, married, divorced)          | `object` |
| `education`      | Education level                                     | `object` |
| `default`        | Has credit in default? (`yes`/`no`)                 | `object` |
| `housing`        | Has housing loan? (`yes`/`no`)                      | `object` |
| `loan`           | Has personal loan? (`yes`/`no`)                     | `object` |
| `contact`        | Type of communication contact                       | `object` |
| `month`          | Last contact month (`jan`, `feb`, …)                | `object` |
| `day_of_week`    | Last contact day of the week                        | `object` |
| `duration`       | Duration of last contact (in seconds)               | `int`    |
| `campaign`       | Number of contacts performed during this campaign   | `int`    |
| `pdays`          | Days passed after last contact (999 means never)    | `int`    |
| `previous`       | Number of contacts before this campaign             | `int`    |
| `poutcome`       | Outcome of previous marketing campaign              | `object` |
| `emp.var.rate`   | Employment variation rate (economic indicator)      | `float`  |
| `cons.price.idx` | Consumer price index                                | `float`  |
| `cons.conf.idx`  | Consumer confidence index                           | `float`  |
| `euribor3m`      | Euribor 3 month rate                                | `float`  |
| `nr.employed`    | Number of employees                                 | `float`  |

---

## ⚠️ Important Notes

* ✅ **No null values** explicitly present.
* 🧹 All **categorical features were label/one-hot encoded** before modeling.
* ⚖️ The dataset is **imbalanced** (more "no" than "yes" in the target), so:

  * Metrics like **Recall**, **F1-Score**, and **AUC** were emphasized.
  * **SMOTE** was applied during training.

---

## 💼 Dataset Usage in Project

📘 Main notebook:

> `notebooks/term_deposit_prediction.ipynb`

🧠 Task Objective:

> Predict whether a customer will **subscribe to a term deposit** after a marketing campaign.

---

