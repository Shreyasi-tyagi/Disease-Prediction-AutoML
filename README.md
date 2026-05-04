# 🏥 Disease Prediction System

### AutoML vs Manual Hyperparameter Tuning

---

## 📌 Overview

This project compares **manual hyperparameter tuning** and **AutoML (TPOT)** for predicting chronic kidney disease using a real-world medical dataset.

The goal is to evaluate which approach provides better performance in terms of accuracy and efficiency.

---

## 🎯 Objective

* Build a disease prediction model
* Compare:

  * Manual tuning (GridSearchCV)
  * AutoML (TPOT)
* Evaluate performance using standard metrics

---

## 📂 Dataset

* **Name:** Chronic Kidney Disease Dataset
* **Records:** 400
* **Features:** 25
* Includes:

  * Numerical (age, bp, bgr, etc.)
  * Categorical (rbc, pc, htn, etc.)

---

## ⚙️ Methodology

### 🔹 Data Preprocessing

* Removed irrelevant column (`id`)
* Handled missing values using **mean imputation**
* Converted object-type numeric columns (`pcv`, `wc`, `rc`)
* Encoded categorical variables
* Applied **feature scaling (StandardScaler)**

---

### 🔹 Train-Test Split

* 80% training / 20% testing
* Used **stratified sampling** to handle class imbalance

---

### 🔹 Models Used

#### 🧑‍💻 Manual Approach

* Random Forest Classifier
* Hyperparameter tuning using **GridSearchCV**

#### 🤖 AutoML Approach

* TPOT (Tree-based Pipeline Optimization Tool)
* Automatically selects best pipeline

---

## 📊 Results

| Model                               | Accuracy  | Precision | Recall | F1 Score |
| ----------------------------------- | --------- | --------- | ------ | -------- |
| Manual (Random Forest + GridSearch) | **0.975** | 0.98      | 0.97   | 0.97     |
| AutoML (TPOT)                       | 0.95      | 0.95      | 0.95   | 0.95     |

---

## 🏆 Key Findings

* Manual tuning slightly outperformed AutoML
* AutoML required more computational resources
* Feature preprocessing significantly impacted results

---

## 💡 Conclusion

> Manual hyperparameter tuning provided better accuracy for this dataset, while AutoML offered automation and ease of use.

This shows that **manual tuning is effective for smaller datasets**, whereas AutoML is useful for larger and more complex problems.

---

## 🛠️ Tech Stack

* Python
* Scikit-learn
* TPOT (AutoML)
* Pandas, NumPy
* Google Colab

---

## 🚀 How to Run

1. Open the notebook in Google Colab
2. Upload the dataset (`kidney_disease.csv`)
3. Run all cells

---


---

## 🔮 Future Work

* Try other AutoML tools
* Improve handling of imbalanced data
* Deploy as a web application

---

## 👩‍💻 Author

Machine Learning Mini Project
