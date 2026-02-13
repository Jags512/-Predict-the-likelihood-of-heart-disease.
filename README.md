# -Predict-the-likelihood-of-heart-disease.

# ❤️ Heart Disease Prediction  
Kaggle Playground Series – February 2026  

## 📌 Problem Statement

The objective of this competition is to predict the **likelihood of heart disease** for each patient based on clinical and demographic features.

This is a **binary classification problem**, where:

- `1` → Patient has heart disease  
- `0` → Patient does not have heart disease  

---

## 📊 Dataset Overview

The dataset includes:

- Demographic attributes
- Medical test measurements
- Clinical indicators
- Target variable: `Heart Disease`
- Unique identifier: `id`

The dataset is synthetically generated for educational and experimentation purposes.

---

## 🎯 Evaluation Metric

The competition is evaluated using:

### 🟢 Area Under the ROC Curve (AUC)

\[
AUC = \text{Area under ROC curve}
\]

- Measures model's ability to distinguish between classes
- Value ranges from 0.5 (random guessing) to 1.0 (perfect classifier)
- Higher AUC indicates better model performance

---

## 🛠️ Approach

### 1️⃣ Data Preprocessing
- Removed `id` column
- Handled missing values using median imputation
- Encoded categorical features using Label Encoding
- Checked class balance
- Performed 5-Fold Stratified Cross Validation

### 2️⃣ Model Used

Primary model:
- **LightGBM Classifier**

Why LightGBM?

- Efficient for large tabular datasets
- Handles non-linear relationships
- Works well with imbalanced data
- Strong Kaggle performance

### 3️⃣ Cross Validation

- Used **Stratified K-Fold (5 folds)** to maintain class distribution
- Applied early stopping to avoid overfitting
- Generated Out-of-Fold (OOF) predictions

---

## 📈 Model Performance

- Cross Validation AUC: `XX.XXXX`
- Evaluation Metric: ROC-AUC

(Replace with your actual CV score)

---

## 🔥 Advanced Techniques Applied

- Stratified Cross Validation
- Feature Importance Analysis
- Probability-based predictions
- Ensemble-ready pipeline structure

---

## 🚀 Future Improvements

- Hyperparameter tuning using Optuna
- Trying CatBoost and XGBoost
- Model ensembling
- Target encoding for categorical variables
- Feature interaction engineering

---

kaggle_link:https://www.kaggle.com/code/jagrutiyuvrajdhangar/heart-diseare-pred/edit

