# 🫀 Heart Disease Prediction using Machine Learning

## ○ Task Objective

The objective of this project is to build a machine learning classification model to predict the presence of heart disease in patients based on medical attributes.

The model analyzes various health indicators such as age, cholesterol level, chest pain type, blood pressure, and heart rate to determine whether a patient is at risk of heart disease.

This is a binary classification problem:
- **0 → No heart disease**
- **1 → Heart disease present**

---

## ○ Dataset Used

The dataset used in this project contains **920 patient records** with **16 medical features** related to heart health.

### Key Features:

- `age` – Age of the patient  
- `sex` – Gender  
- `cp` – Chest pain type  
- `trestbps` – Resting blood pressure  
- `chol` – Serum cholesterol level  
- `fbs` – Fasting blood sugar  
- `thalch` – Maximum heart rate achieved  
- `exang` – Exercise induced angina  
- `oldpeak` – ST depression induced by exercise  
- `ca` – Number of major vessels  
- `thal` – Thalassemia  

### Data Preprocessing Steps:

- Handled missing values
- Encoded categorical variables using One-Hot Encoding
- Converted multi-class target into binary classification
- Removed irrelevant columns (e.g., `id`) to prevent data leakage
- Split dataset into training and testing sets

---

## ○ Models Applied

### 🌳 Decision Tree Classifier

The Decision Tree model was selected because:

- It works well for classification problems
- It does not require feature scaling
- It provides feature importance for interpretation
- It is easy to visualize and understand

The model was trained on the training dataset and evaluated on the test dataset.

---

## ○ Key Results and Findings

### 📊 Model Performance

- **Accuracy:** 72%
- **Precision (Heart Disease):** 79%
- **Recall (Heart Disease):** 72%
- **F1-Score:** 75%

### 🔍 Confusion Matrix Summary

- 79 heart disease cases correctly predicted
- 54 healthy cases correctly predicted
- Some false positives and false negatives observed

### ⭐ Most Important Features

According to feature importance analysis, the top predictors were:

- `chol` (Cholesterol)
- `cp` (Chest pain type)
- `age`
- `thalch` (Maximum heart rate)
- `oldpeak` (ST depression)

### 🧠 Key Insights

- Cholesterol level and chest pain type are strong indicators of heart disease.
- Removing the `id` column significantly improved model reliability by preventing data leakage.
- The model performs reasonably well but could be further improved using ensemble methods like Random Forest or Gradient Boosting.

---

## 📌 Conclusion

The Decision Tree model achieved satisfactory performance in predicting heart disease risk with 72% accuracy.  

This project demonstrates a complete machine learning workflow including:

- Data cleaning  
- Feature encoding  
- Model training  
- Performance evaluation  
- Feature importance interpretation  

Future improvements may include hyperparameter tuning and testing more advanced ensemble models.

---

## 🚀 Technologies Used

- Python  
- Pandas  
- NumPy  
- Scikit-learn  
- Matplotlib  
- Seaborn  

---



