# 🧠 ML - Cerebral Stroke Prediction (Imbalanced Data)
This project focuses on building a machine learning model to predict the likelihood of a cerebral stroke using medical and demographic data. The dataset is highly imbalanced, making it a great example for practicing classification techniques and handling skewed data.

# 📌 Problem Statement
Cerebral stroke is a major health concern, and early prediction can help in timely intervention. However, stroke events are rare, leading to a class imbalance where most patients do not have a stroke. This project addresses the challenge of predicting stroke occurrences in such imbalanced data.

# 📁 Dataset Overview
The dataset includes the following features:

Demographics: gender, age, hypertension, heart_disease, ever_married, work_type, Residence_type

Health metrics: avg_glucose_level, bmi, smoking_status

Target: stroke (0 = No stroke, 1 = Stroke)

# 🔍 Exploratory Data Analysis (EDA)
Checked class imbalance: stroke cases are < 5% of the dataset.

Visualized feature distributions for stroke vs. non-stroke groups.

Identified missing values and patterns (e.g., in bmi and smoking_status).

# ⚙️ Data Preprocessing & Imbalance Handling
Missing values: Imputed using mean/mode.

Categorical encoding: Label encoding and one-hot encoding where necessary.

Balancing techniques:

Applied SMOTE (Synthetic Minority Over-sampling Technique).

Compared with Random Undersampling.

# 🤖 Models Trained
Logistic Regression

Random Forest Classifier

Support Vector Machine (SVM)

XGBoost Classifier

# 📊 Evaluation Metrics:
Due to class imbalance, we used:

Precision, Recall, F1-Score

Confusion Matrix

ROC-AUC Score

# 🏁 Conclusion
XGBoost and Random Forest gave the best results with SMOTE.

Using ROC-AUC and F1-score helped evaluate performance better than just accuracy.

Feature importance showed that age, avg_glucose_level, and hypertension were the top predictors.

# 🛠️ Tools & Libraries
Python, Pandas, NumPy, Seaborn, Matplotlib

Scikit-learn

Imbalanced-learn (imblearn)

XGBoost

