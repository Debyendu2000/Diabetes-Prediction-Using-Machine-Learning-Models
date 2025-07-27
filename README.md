# 🩺 Diabetes Prediction using Classification Models

This machine learning project focuses on **predicting diabetes** using various classification models. The goal is to compare different algorithms and select the most effective one for accurate binary classification (Diabetic or Non-Diabetic).

---

## 📌 Objective

To build predictive models that can classify patients as **Diabetic** or **Non-Diabetic** based on health-related features from a dataset.

---

## 📂 Dataset

The dataset includes features like:
- Pregnancies
- Glucose
- Blood Pressure
- Skin Thickness
- Insulin
- BMI
- Diabetes Pedigree Function
- Age

**Target column**:  
- `0` → Non-Diabetic  
- `1` → Diabetic

---

## 🔍 Project Highlights

### ✅ Models Used
- **Support Vector Machine (SVM)**
  - Kernels: Linear, RBF, Polynomial, Sigmoid
- **Decision Tree Classifier**
- **Random Forest Classifier**
- **K-Nearest Neighbors (KNN)**
- **Voting Classifier (Ensemble)**
  - Soft Voting

---

## 🧪 Evaluation Metrics

Each model is evaluated using:
- Accuracy (Training & Testing)
- Confusion Matrix
- Precision, Recall, F1-Score
- ROC Curve and AUC Score (for probabilistic models)

---

## 📊 Visualizations

- Confusion matrix heatmaps
- ROC curves
- Classification report heatmaps
- Elbow curve for KNN

---

## ⚙️ Preprocessing Steps

- **Data Cleaning**: Handling zero values for features like Insulin, Skin Thickness
- **Standardization**: Used `StandardScaler`
- **Dimensionality Reduction**: PCA (for visualizing decision boundaries and noise reduction)
- **Nan-Value Checking**
- **Data Visualization** : Data has been visualized projecting in lower dimensional space leveraging **PCA**
  

---

## 📈 KNN Specifics

- Optimal `k` value selected using **Elbow Method**
- Error rate plotted against `k` values (1 to 50)

---

## 🧠 Voting Classifier

Combined predictions from:
- SVM (with `probability=True`)
- Decision Tree
- Logistic Regression
- KNN
- Random Forest

Voting strategies:
- **Soft Voting**: Weighted average of predicted probabilities

---

## 📦 Installation

### Requirements
```bash
pip install -r requirements.txt
