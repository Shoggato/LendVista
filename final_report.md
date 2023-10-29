## Overview of the Analysis
The financial information that we utilized were loan statuses, so if they are high-risk (1) or healthy loans (0).  The prediction will be whether a loan will be classified between these two options. The variables that are being used to predict are float/integers.  The machine learning parts started with seperating the the features, in this case 'loan_status' and the labels which is all the other columns in the dataframe lending_data.  The next step will be to split the data randomly between training features/labels, and testing features/labels.  This will be done with train_test_split function.  finally training a logistic regression model by .fit()ing the training features and the training labels.  Then utilizing .predict() on the newly trained model the features from the testing to see how well the model performs with data it has never seen before. LogisticRegression() model from scikit learn was utilized to form a best fit line for a binary classification model.  Once the regression model has been trained, it is easy to make predictions following the R line.

## Results

Using bulleted lists, describe the accuracy scores and the precision and recall scores of all machine learning models.

* Machine Learning Model 1:
  <ul>
    <li>Accuracy: 99%</li>
    <li>Precision: 1.00 (100%)</li>
    <li>Recall: 0.99 (99%)</li>
  </ul>

* Machine Learning Model 2:
  <ul>
      <li>Accuracy: 99%</li>
      <li>Precision: 0.85 (85%)</li>
      <li>Recall: 0.91 (91%)</li>
    </ul>

## Summary

The predictive model for healthy loans (0) performed the best while high-risk loans (1) didn't perform as well.  This can be seen between the f1-scores, the healthy loans f1-score was 1.00 which is the best you can possibly ask for.  While high-risk loans had an f1-score of 0.88, which isn't so bad, however, when dealing with loans, the precision for high-risk models missed 15% of the actual high-risk loans.  This will lead to more higher-risk loans being approved if using this predictive model which could lead to more defaulted loans costing the loan company excess money.

I do not recommend the high-risk loan (1) predictive model as its f1-score is not greater than 0.95.  The model will miss 15% of the total high-risk loans.  This too me seems a little too steep, and will cost the loan company alot of money if allowed to go into final production.  A different predictive model should be used, or a larger data set of high-risk loans to more effectively train the model.
