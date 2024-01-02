# Project: LendVista
# Loan Risk Prediction

## Overview
The Loan Risk Prediction project utilizes logistic regression to assess the health of loans based on various features. The goal is to predict whether a loan is healthy or high-risk.

## Usage
1. **Data Preparation:**
   - Import data from `lending_data.csv` in the Resources folder.
   - Split data into labels (y) and features (X).

2. **Training and Testing:**
   - Split data into training and testing sets using `train_test_split`.
   - Create a Logistic Regression model using `LogisticRegression` from SKLearn.

3. **Model Evaluation:**
   - Generate a confusion matrix and print a classification report for model performance.

## Results
- The model excels in predicting healthy loans (0) with high precision and recall.
- Performance is slightly lower for high-risk loans (1), indicating room for improvement.

## Dependencies
- Python libraries: NumPy, Pandas, Matplotlib, Scikit-Learn.

## Author
Erika Walker

## License
This project is licensed under the MIT License - see the LICENSE.md file for details.
