## Diabetes Prediction Analysis (Project)
(Models Used : RandomForestClassifier , LightGBM)

This project performs Exploratory Data Analysis (EDA) on a medical dataset to identify key factors contributing to diabetes.

## 1. Understanding the Problem & the Dataset

The project addresses a critical healthcare question "Which factors most accurately make a diabete happen?"

To answer that, I analyzed a dataset and examined:

- Demographic distributions (Age, Gender).

- Clinical indicators (BMI, HbA1c level, Blood Glucose level).

- Existing medical conditions (Hypertension, Heart Disease).

- Lifestyle factors (Smoking history).

## 2. Exploratory Data Analysis (EDA)

Using Python in a Jupyter Notebook, I performed a detailed exploration of the healthcare data:

- Visualized the distribution of glucose levels across different age groups.

- Investigated the correlation between BMI and diabetes prevalence.

- Assessed data types and verified the structure of the 100,000 records.

- Analyzed the imbalance between diabetic and non-diabetic samples.

## 3. Data Cleaning & Feature Engineering

Before modeling, I cleaned the dataset to ensure better inputs for analysis

- Duplicate Management

Identified and removed 3,854 duplicate entries to prevent model bias.

- Data Formatting

Checked feature types (integers, floats, and objects) for compatibility with analytical libraries.

- Feature Preparation

Prepared key predictors such as HbA1c levels and Blood Glucose levels, which are primary indicators for diabetic classification.

## 4. Machine Learning Models

I implemented two high-performance classifiers to predict diabetes risk, specifically optimizing for F1-Score and PR-AUC to handle the imbalanced nature of the medical data

- Random Forest Classifier: A robust ensemble method used to identify high-risk patients through decision tree aggregation and hyperparameter tuning.

- LightGBM (Light Gradient Boosting Machine): An efficient gradient boosting framework tuned via RandomizedSearchCV to maximize prediction speed and accuracy on the 100,000-record dataset.

## 5. Model Evaluation

To compare the performance of both models fairly, I used the following metrics:

- Accuracy & F1-Score: To measure the overall correctness and balance between precision and recall.

- PR-AUC (Precision-Recall Area Under Curve): Specifically used to compare RandomForest vs. LightGBM in handling the imbalanced nature of the dataset.

- Confusion Matrix: To visualize true positives and false negatives, which is crucial for medical diagnosis.

## 6. Health Insights from the Analysis

The analysis provided valuable medical insights:

- Compared the PR-AUC scores of both models to determine which framework is more reliable for screening.

- Identified that HbA1c and Blood Glucose are the most significant predictors in both models.

- Recommended using LightGBM for larger-scale clinical applications due to its superior efficiency.

## 7. Tools & Technologies Used

- Python (VS Code / Jupyter)

- Pandas & NumPy: For data cleaning and manipulation.

- Matplotlib & Seaborn: For clinical data visualization and PR-curve plotting.

- Scikit-Learn: For the RandomForest model and hyperparameter optimization.

- LightGBM: For the advanced gradient boosting model.

---
