# Model based on loan risk
I use a dataset of historical lending activity from a peer-to-peer lending services company to build a model that can identify the creditworthiness of borrowers.

# Instructions

The instructions for this Challenge are divided into the following subsections: 
* Split the Data into Training and Testing Sets
* Create a Logistic Regression Model with the Original Data
* Write a Credit Risk Analysis Report

Create the labels set (y) from the “loan_status” column, and then create the features (X) DataFrame from the remaining columns.
Fit a logistic regression model by using the training data (X_train and y_train).
Save the predictions for the testing data labels by using the testing feature data (X_test) and the fitted model.

**Question:** How well does the logistic regression model predict both the `0` (healthy loan) and `1` (high-risk loan) labels?

**Answer:** The logistic regression model fit with the oversampled data performed the same when predicting the "healthy loan" label, with perfect precision and F1 score, and nearly perfect recall. For the "high-risk loan" data, the precision was 1% lower for the resampled data, but the recall was 8% higher, and the F1 score was 3% higher. Overall, the model performed better with the resampled data than with the imbalanced data.
