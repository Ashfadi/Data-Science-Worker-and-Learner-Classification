# Data Science Worker and Learner Classification

## Overview
This project analyzes and classifies data science workers and learners based on their yearly salary. The classification task aims to predict whether an individual earns more than $100K annually, using various features such as experience, education, and tools used.

---

## Objectives
1. Preprocess raw datasets into a format suitable for machine learning models.
2. Explore and clean the data to handle missing values and categorical attributes.
3. Apply classification models using Python's `scikit-learn` library to predict salary categories.
4. Compare different models for performance evaluation.

---

## Tools and Technologies
- **Programming Language**: Python
- **Libraries**:
  - `pandas` for data preprocessing.
  - `scikit-learn` for machine learning.
  - `numpy` for numerical computations.
- **Visualization Tools**: Decision tree visualization using `.dot` files.

---

## Dataset Details
- **Files**:
  - `ds_workers_learners.csv`: Original dataset with multiple columns and over 3000 rows.
  - `small_ds_workers_learners.csv`: Simplified dataset with fewer columns for exploration.
  - `p3_processed.csv`: Preprocessed dataset ready for classification tasks.
- **Key Features**:
  - `Yearly Salary`: Binary classification target (`Yes` for >$100K, `No` otherwise).
  - `Years of Experience in Machine Learning`: Ordinal feature.
  - `Tools Used`: Encoded nominal feature via one-hot encoding.

---

## Key Tasks and Steps

### **1. Data Preprocessing**
- Handled missing values by:
  - Dropping rows with null target values.
  - Replacing nulls in categorical features with appropriate default values (`0` or "None").
- Applied transformations:
  - Converted salary into binary categories (`Yes`/`No`).
  - One-hot encoded nominal attributes such as `Tools Used`.
  - Ordinally encoded features like `Experience in Machine Learning`.

### **2. Model Training**
- Built multiple classifiers:
  - **Decision Tree Classifier**: Visualized using a `.dot` file.
  - **Multinomial Naive Bayes Classifier**
  - **K-Nearest Neighbors (KNN) Classifier**
- Used 5-fold cross-validation for performance evaluation.

### **3. Model Evaluation**
- Evaluated models using:
  - Confusion Matrix
  - Classification Report (Precision, Recall, F1-Score)
  - Accuracy on the test set.
- Example output:
  - Decision Tree Accuracy: **75%**
  - Multinomial Naive Bayes Accuracy: **76%**
