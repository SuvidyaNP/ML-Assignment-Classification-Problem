# ML-Assignment-Classification-Problem

# Breast Cancer Classification

This project implements various classification algorithms on the Breast Cancer dataset available in the `sklearn` library. The goal is to compare the performance of different algorithms and determine the best classifier for this dataset.

---

## **1. Dataset and Preprocessing**

- **Dataset**: The Breast Cancer dataset from the `sklearn` library.
- **Preprocessing Steps**:
  1. **Missing Values**: Handled using the mean imputation strategy. No missing values were present in this dataset.
  2. **Feature Scaling**: Standardized all features using `StandardScaler` to ensure algorithms like SVM and k-NN perform optimally.
  3. **Splitting**: Divided the dataset into training and testing sets using an 80-20 split.

---

## **2. Classification Algorithms**

The following classification algorithms were implemented:

1. **Logistic Regression**
   - A linear model that predicts the probability of a binary outcome using a logistic function.
   - Achieved the **highest accuracy (97%)**, likely due to the linear separability of the data.

2. **Decision Tree Classifier**
   - A non-linear algorithm that splits data into subsets based on feature thresholds.
   - Accuracy: **95%**. It may have slightly overfitted the data.

3. **Random Forest Classifier**
   - An ensemble method that uses multiple decision trees and averages their results.
   - Accuracy: **96%**. Robust to overfitting and effective on this dataset.

4. **Support Vector Machine (SVM)**
   - Finds the optimal hyperplane that separates classes with maximum margin.
   - Accuracy: **96%**. Performed well due to feature scaling.

5. **k-Nearest Neighbors (k-NN)**
   - Classifies samples based on their nearest neighbors in the feature space.
   - Accuracy: **95%**. Sensitive to the choice of `k` and data scaling.

---

## **3. Model Comparison**

The performance of the algorithms is summarized below:

| Algorithm             | Accuracy |
|-----------------------|----------|
| Logistic Regression   | 97%   |
| Random Forest         | 96%   |
| Support Vector Machine| 96%   |
| Decision Tree         | 95%   |
| k-NN                  | 95%   |
