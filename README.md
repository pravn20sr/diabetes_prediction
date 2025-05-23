# 🩺 Diabetes Prediction Using Machine Learning Models

This project aims to classify individuals as diabetic or non-diabetic using health-related data and machine learning algorithms. It utilizes the **Pima Indians Diabetes Dataset** from [Kaggle](https://www.kaggle.com/datasets/akshaydattatraykhare/diabetes-dataset/data) and applies various data science techniques to build an accurate and reliable model.

---
## 🧠 Objective

To build a predictive model that can accurately identify whether a person is diabetic based on diagnostic health data, enabling early intervention and better health management.

---
## 📂 Dataset

- **Source:** [Kaggle - Diabetes Dataset](https://www.kaggle.com/datasets/akshaydattatraykhare/diabetes-dataset/data)
- **Features:**
  - Pregnancies
  - Glucose
  - Blood Pressure
  - Skin Thickness
  - Insulin
  - BMI
  - Diabetes Pedigree Function
  - Age
- **Target:** Outcome (0 = Non-Diabetic, 1 = Diabetic)

---
## 🛠️ Technologies Used

- 🐍 Python
- 📘 Pandas, NumPy
- 📊 Matplotlib, Seaborn
- 🤖 Scikit-learn

---
## 🔄 Project Workflow
- **Data Collection and Loading:** Load the dataset and perform initial inspections using Pandas.
- **Exploratory Data Analysis (EDA):** Analyze trends, visualize distributions, identify correlations, and examine the class imbalance in the target variable.
- **Data Preprocessing:**
   - Handle missing or zero values in key features.
   - Normalize and scale numerical columns.
   - Apply **SMOTE (Synthetic Minority Over-sampling Technique)** to balance the dataset by generating synthetic samples for the minority class (diabetic cases).
- **Model Building:** Train multiple classification models, including:
   - Logistic Regression
   - Random Forest
   - Decision Tree
   - XGBoost
- **Model Evaluation and Tuning:** Evaluate performance using metrics like **Accuracy**, **Precision**, **Recall**, **F1-score**. Apply **GridSearchCV** to fine-tune hyperparameters for optimal results.
---
## 📈 Results Summary
- **Best Performing Model:** Logistic Regression
- **Accuracy:** `76%`
- **Precision:** `62%`
- **Recall:** `83%`
- **F1 Score:** `71%`

**Main takeaways:** 
- Good Overall Accuracy: The model achieved an accuracy of 76%, indicating it performs well in correctly classifying diabetic and non-diabetic cases in the test dataset.
- High Recall for Diabetic Cases: With a recall of 83%, the model is effective at identifying actual diabetic patients, minimizing the risk of missing true positive cases — which is crucial in healthcare scenarios.
- Precision: The model's precision of 62% suggests that some non-diabetic cases are being falsely predicted as diabetic, which could lead to unnecessary follow-ups but is often acceptable in early screening models where catching true positives is a priority.
- Balanced Performance (F1 Score): An F1 Score of 0.71 shows a good balance between precision and recall, making this model suitable for practical use where both false positives and false negatives have significant impacts.
