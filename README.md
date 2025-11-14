# Heart Disease Prediction using Logistic Regression

# Project Overview
This project aims to **predict whether a patient has heart disease** using **Logistic Regression**, a supervised machine learning algorithm.

# Dataset Description

The dataset (heart_disease_dataset.csv) contains patient health-related attributes such as:
- Gender
- Age
- Smoking
- Alcohol Intake
- Family History
- Diabetes
- Obesity
- Exercise Induced Angina
- Chest Pain Type
- Exercise Hours
- Cholesterol
- Heart Disease (Target: 1 = Yes, 0 = No)

# Steps Performed

# 1.Technologies Used
- Python  
- Pandas  
- NumPy  
- Matplotlib  
- Scikit-learn  
- Jupyter Notebook
  
# 2. Loaded the Dataset
- Read heart_disease_dataset.csv using Pandas.
- Checked for missing values with df.isnull().sum().

# 3. Encoded Categorical Features
Converted categorical columns into numerical codes:
- Gender
- Smoking
- Alcohol Intake
- Family History
- Diabetes
- Obesity
- Exercise Induced Angina
- Chest Pain Type

# 4. Handled Invalid & Missing Values
- Replaced -1 in Alcohol Intake with NaN.
- Removed missing rows using df.dropna().

# 5. Prepared Features and Target
- X = all columns except 'Heart Disease'
- y = 'Heart Disease'

# 6. Train-Test Split
Split data into 80% training and 20% testing using train_test_split().

# 7. Built Logistic Regression Model
Created and trained the model using:
model = LogisticRegression()
model.fit(X_train, y_train)

# 8. Made Predictions
Generated predictions using model.predict(X_test).

# 9. Evaluated the Model
Calculated accuracy using accuracy_score(y_test, y_predict).

# 10. Performed Data Visualizations
- Scatter plot (Age vs Heart Disease)
- Cholesterol histogram
- Gender-wise bar chart
- Age distribution histogram
- Exercise Hours vs Heart Disease bar chart
- Gender distribution pie chart
 
# Results
- Accuracy check

# Structure
```
project/
│── heart_disease_dataset.csv
│── project.ipynb
│── README.md
```
