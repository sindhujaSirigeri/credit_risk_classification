# credit_risk_classification

# Loan Risk Classification Project

This project uses logistic regression to classify loans as either "Healthy Loan" (label 0) or "High-Risk Loan" (label 1). The model is trained on a dataset containing loan information, and its performance is evaluated using various metrics.

## Table of Contents

-   [Introduction](#introduction)
-   [Dataset](#dataset)
-   [Installation](#installation)
-   [Usage](#usage)
-   [Results](#results)
-   [Skills Used](#skills-used)
-   [Contributing](#contributing)
-   [License](#license)

## Introduction

The primary goal of this project is to develop a reliable model to predict the risk associated with loans. By accurately identifying high-risk loans, financial institutions can minimize losses and make informed lending decisions.

## Dataset

The dataset used in this project contains information about loans, including the `loan_status` column, which indicates whether a loan is healthy or high-risk. The dataset is stored in a CSV file named `lending_data.csv`.

## Usage

1.  Ensure the dataset (`lending_data.csv`) is placed in the `Resources` folder.
    
2.  Run the Jupyter Notebook or Python script to train the model and evaluate its performance.
    
3.  The model will output a confusion matrix, classification report, and key metrics such as precision, recall, and F1-score.


## Machine Learning Process

1.  **Describing the Data:** Analyzing and understanding the dataset’s structure and content.
2.  **Identifying Correlations:** Examining correlations between features to understand relationships and multicollinearity.
3.  **Checking Linearity:** Assessing linearity between the labels and the target variable to validate logistic regression assumptions.
4.  **Separating Data:** Splitting the data into labels (`y`) and features (`X`).
5.  **Splitting Data:** Dividing the data into training and testing datasets.
6.  **Instantiating the Model:** Creating a logistic regression model.
7.  **Fitting the Model:** Training the model with the training dataset.
8.  **Predicting Results:** Using the model to predict outcomes on the testing dataset.
9.  **Evaluating the Model:** Generating and analyzing the confusion matrix and classification report to assess performance.

## Results

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

In summary, the logistic regression model performs exceptionally well in predicting both healthy and high-risk loans. It demonstrates high precision, recall, and accuracy, making it a reliable model for this classification task. While precision, accuracy, and F1-score are high, recall is considered the most crucial parameter for evaluating the model's overall performance. It highlights the model's ability to correctly identify both healthy and high-risk loans, which is essential for establishing the model's credibility and effectiveness in classifying loan risks.

## Skills Used

-   **Python Programming:** Utilized for data manipulation, model training, and evaluation.
-   **Pandas:** For data preprocessing and analysis.
-   **Scikit-learn:** For machine learning model implementation, including logistic regression and evaluation metrics.
-   **Jupyter Notebook:** For interactive data exploration and analysis.
-   **Data Visualization:** Used to display the confusion matrix and other metrics.