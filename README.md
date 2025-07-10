# 🧠 Diabetes Prediction using SVM

## 📌 Project Overview

This project involves predicting the likelihood of diabetes using the Support Vector Machine (SVM) algorithm. The dataset was sourced from Kaggle, and the full machine learning pipeline was implemented in Google Colab.

---

## 🔧 Steps Performed

### 1️⃣ Dataset

* Used `diabetes_prediction_dataset.csv` from Kaggle
* Target column: `diabetes` (0 = No, 1 = Yes)
* Uploaded to GitHub and loaded via raw link

### 2️⃣ Preprocessing

* One-hot encoded categorical features (`gender`, `smoking_history`)
* Split into train/test sets using an 80/20 ratio
* Applied feature scaling using `StandardScaler` (important for SVM)

### 3️⃣ Model Training

* Trained `SVC()` model from `sklearn.svm`
* Evaluation metrics:

  * Accuracy
  * Precision
  * Recall
  * F1-score
  * Specificity
  * Confusion matrix

### 4️⃣ Hyperparameter Tuning

* Used `GridSearchCV` with 5-fold cross-validation
* Tuned parameters:

  * `C` (regularization strength)
  * `gamma` (kernel coefficient)
  * `kernel` (`rbf`, `linear`)
* Re-evaluated the model using the best estimator

---

## ✅ Final Evaluation

The tuned SVM model performed well and effectively handled class imbalance. **Specificity** was particularly useful for accurately detecting non-diabetic cases.
