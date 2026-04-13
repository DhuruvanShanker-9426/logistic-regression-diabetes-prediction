# 🩺 Diabetes Prediction using Logistic Regression

---

## 📊 Project Overview

This project builds a **machine learning classification model** using Logistic Regression to predict whether a person has diabetes based on medical features.

The model is trained on the **Pima Indians Diabetes Dataset**, a widely used dataset for binary classification problems.

---

## 🎯 Objectives

* Understand and implement Logistic Regression
* Perform Exploratory Data Analysis (EDA)
* Clean and preprocess real-world data
* Evaluate model performance using multiple metrics
* Improve model performance using threshold tuning

---

## 🛠️ Tools & Technologies

* Python 🐍
* Pandas
* NumPy
* Matplotlib
* Seaborn
* Scikit-learn

---

## 📂 Dataset Information

The dataset contains the following features:

* Pregnancies
* Glucose
* Blood Pressure
* Skin Thickness
* Insulin
* BMI
* Diabetes Pedigree Function
* Age

🎯 Target Variable:

* **Outcome (0 = No Diabetes, 1 = Diabetes)**

---

## ⚙️ Project Workflow

### 🔹 1. Data Preprocessing

* Handled invalid zero values in important features
* Cleaned and prepared dataset for modeling

---

### 🔹 2. Exploratory Data Analysis (EDA)

* Univariate analysis for distribution understanding
* Bivariate analysis for relationship insights

---

### 🔹 3. Model Building

* Applied **Logistic Regression**
* Split data into training and testing sets
* Trained model on training data

---

### 🔹 4. Model Evaluation

* Accuracy
* Precision
* Recall
* F1 Score
* Confusion Matrix
* ROC-AUC Score

---

## 📈 Model Performance

### 🔹 Before Threshold Tuning (Default = 0.5)

* Accuracy: **0.7532**
* Precision: **0.6923**
* Recall: **0.5094**
* F1 Score: **0.5869**
* ROC-AUC Score: **0.6953**

📌 Confusion Matrix:

```
[[89 12]
 [26 27]]
```

---

### 🔹 After Threshold Tuning (Threshold = 0.3)

* Accuracy: **0.7792**
* Precision: **0.6557**
* Recall: **0.7547**
* F1 Score: **0.7018**
* ROC-AUC Score: **0.7734**

📌 Confusion Matrix:

```
[[80 21]
 [13 40]]
```

---

## 🧠 Key Insights

* Reducing the threshold from **0.5 to 0.3** significantly improved **Recall (0.51 → 0.75)**
* The model became better at identifying diabetic patients (**reduced false negatives**)
* Slight drop in Precision is acceptable for medical use cases
* Improved **F1 Score and ROC-AUC**, indicating better overall performance

---

## ⚖️ Trade-off Explanation

* **Before tuning**:

  * Missed many diabetic cases (high False Negatives ❌)

* **After tuning**:

  * Captured more diabetic cases ✅
  * Slight increase in False Positives ⚠️

👉 In healthcare applications, **Recall is more important than Precision**, making this trade-off beneficial.

---

## 🚀 Key Highlights

* Built an end-to-end **Machine Learning classification model**
* Performed **EDA → Preprocessing → Modeling → Evaluation**
* Applied **threshold tuning** to improve model performance
* Compared metrics before and after optimization

---

## 📷 Model Output

### 🔹 Before Threshold Tuning
<img src="https://i.postimg.cc/SKc7WzNZ/cm-before-updating-threshold.png" width="600">

### 🔹 After Threshold Tuning
<img src="https://i.postimg.cc/6QCgyqsN/cm-after-updating-threshold.png" width="600">

---

## 📚 What I Learned

* Working of Logistic Regression in real-world problems
* Importance of data preprocessing
* Model evaluation using multiple metrics
* Trade-off between Precision and Recall
* Practical use of threshold tuning

---

## 🔗 Future Improvements

* Apply advanced models (Random Forest, XGBoost)
* Hyperparameter tuning
* Feature engineering
* Deploy using Streamlit

---

## 📌 Conclusion

This project demonstrates a strong understanding of **machine learning classification** and shows how model performance can be improved using **threshold tuning techniques**, making it more suitable for real-world applications.
