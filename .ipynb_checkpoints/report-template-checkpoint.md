# Module 12 Report Template

## Overview of the Analysis

In this section, describe the analysis you completed for the machine learning models used in this Challenge. This might include:

## Goal
<!-- * Explain what financial information the data was on, and what you needed to predict. -->
- The primary goal of this project is to develop a reliable model to predict the risk associated with loans. By accurately identifying high-risk loans, financial institutions can minimize losses and make informed lending decisions.

## Dataset
<!-- * Provide basic information about the variables you were trying to predict (e.g., `value_counts`). -->
* The dataset used in this project contains information about loans, including the `loan_status` column, which indicates whether a loan is healthy or high-risk. The dataset is stored in a CSV file named `lending_data.csv`.

## Machine Learning Process
<!-- * Describe the stages of the machine learning process you went through as part of this analysis. -->
1.  **Describing the Data:** Analyzing and understanding the dataset’s structure and content.
2.  **Identifying Correlations:** Examining correlations between features to understand relationships and multicollinearity.
3.  **Checking Linearity:** Assessing linearity between the labels and the target variable to validate logistic regression assumptions.
4.  **Separating Data:** Splitting the data into labels (`y`) and features (`X`).
5.  **Splitting Data:** Dividing the data into training and testing datasets.
6.  **Instantiating the Model:** Creating a logistic regression model.
7.  **Fitting the Model:** Training the model with the training dataset.
8.  **Predicting Results:** Using the model to predict outcomes on the testing dataset.
9.  **Evaluating the Model:** Generating and analyzing the confusion matrix and classification report to assess performance.

<!-- * Briefly touch on any methods you used (e.g., `LogisticRegression`, or any other algorithm). -->
- The logistic regression model performs exceptionally well in predicting both healthy and high-risk loans. It demonstrates high precision, recall, and accuracy, making it a reliable model for this classification task.

## Results
<!-- Using bulleted lists, describe the accuracy scores and the precision and recall scores of all machine learning models.

* Machine Learning Model 1:
    * Description of Model 1 Accuracy, Precision, and Recall scores. -->
The logistic regression model achieved the following results:

**Label 0 - Healthy Loan**

* Precision: 1.0, meaning the model is 100% accurate when predicting a loan as healthy.
* Recall: 0.99, indicating the model correctly identifies 99% of actual healthy loans.
* F1-score: 1, showing perfect model performance for this class.


**Label 1 - High-Risk Loan**

* Precision: 0.85, meaning the model is correct 85% of the time when predicting a loan as high-risk.
* Recall: 0.91, indicating the model correctly identifies 91% of actual high-risk loans.
* F1-score: 0.88, reflecting an overall good performance.

In summary, the logistic regression model excels in predicting both healthy and high-risk loans, with high precision, recall, and F1-scores, making it a reliable model for this classification task. These results demonstrate the model's high accuracy and reliability in predicting loan risk.

## Summary
<!-- Summarise the results of the machine learning models, and include a recommendation on the model to use, if any. For example:

* Which one seems to perform best? How do you know it performs best?
* Does performance depend on the problem we are trying to solve? (For example, is it more important to predict the `1`'s, or predict the `0`'s? )

If you do not recommend any of the models, please justify your reasoning.
 -->
 The machine learning models were evaluated to classify loans as either healthy or high-risk. Among the models tested, the logistic regression model performed the best. It achieved high accuracy, precision, and recall scores, particularly excelling in identifying high-risk loans with a recall of 0.91. This indicates the model is effective in capturing a high percentage of actual high-risk loans.

Performance is crucially dependent on the problem at hand. For this classification task, accurately predicting high-risk loans (label 1) is more important than predicting healthy loans (label 0), as missing high-risk loans can have significant financial implications. The logistic regression model's balance of precision and recall makes it the preferred choice for this task, as it effectively identifies both healthy and high-risk loans while minimizing errors.