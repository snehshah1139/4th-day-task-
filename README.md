# Internship Task 4: Logistic Regression - Health Insurance Claim Prediction

## Objective
Build a binary classification model using Logistic Regression to predict whether an individual is likely to file a health insurance claim, based on attributes like age, BMI, smoking status, and charges.

---

## Dataset Overview
The dataset includes the following features:

- `age`: Age of the individual  
- `sex`: Gender  
- `bmi`: Body Mass Index  
- `children`: Number of children  
- `smoker`: Smoking status (yes/no)  
- `region`: Residential area  
- `charges`: Medical charges billed  
- `insuranceclaim`: Target variable (1: Claim filed, 0: No claim)  

---

## Project Workflow

### 1. Data Loading and Preprocessing
- Loaded the dataset using Pandas.
- Verified the data for null or missing values.
- Categorical features were already encoded and ready for modeling.

### 2. Exploratory Data Analysis (EDA)
- Analyzed distributions of features using histograms and boxplots.
- Studied correlations between variables using a heatmap.
- Identified that smoking status, BMI, and charges were strongly related to insurance claims.

### 3. Feature Scaling
- Applied `StandardScaler` to normalize the feature set.
- Ensured all input features had zero mean and unit variance.
- Scaling was necessary for logistic regression to perform optimally.

### 4. Model Building and Training
- Implemented Logistic Regression using Scikit-learn.
- Split the dataset into training and testing sets in an 80:20 ratio.
- Trained the model on the scaled features.

### 5. Model Evaluation
- Accuracy Score: 88%
- Confusion Matrix showed strong performance with high true positives and true negatives.
- Classification Report:
  - Precision (claim): 0.93
  - Recall (claim): 0.87
  - F1-Score (claim): 0.90
- ROC-AUC Score: 0.91, indicating good distinction between classes.

### 6. Threshold Tuning and Sigmoid Function
- Logistic Regression produces probabilities using the sigmoid function.
- Demonstrated how changing the classification threshold affects metrics like precision and recall.
- Highlighted its importance in use cases where false positives or false negatives have different business impacts.

---

## Visualizations Included
- Exploratory data plots
- Correlation heatmap
- Confusion matrix
- ROC curve
- Threshold vs Precision/Recall plot (optional)

---

## Final Analysis
The logistic regression model built in this task delivers high accuracy and interpretability. It performs well in classifying insurance claim predictions and is supported by strong evaluation metrics. With careful threshold tuning and feature understanding, this model can be confidently applied to real-world scenarios in the insurance domain.

---

## Tools Used
- Python
- Pandas, NumPy
- Matplotlib, Seaborn
- Scikit-learn
- Google Colab

---


