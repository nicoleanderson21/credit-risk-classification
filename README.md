## Credit-risk-classification

# Overview of the Analysis

The purpose of this analysis was to assess loan risk in order to identify the creditworthiness of borrowers. The financial information used to train the model consisted of loan size, interest rate, borrower income, debt to income, number of accounts, derogatory marks, and total debt. Using this information, the model was trained to predict whether a loan was healthy or high-risk. The training data consisted of 18765 healthy loans and 619 high-risk loans. The data was split into training and testing datasets before being fed to the model. Given the binary outcome, a logistic regression model was used to predict the probability of whether or not a loan was risky.  

# Results

* Logistic Regression Model:
    * Accuracy Score: 99%
    * Precision:
         Healthy loans: 100%
         High-risk loans: 85%
    * Recall:
         Healthy loans: 99%
         High-risk loans: 91%
    * F1-Scores:
         Healthy loans: 100%
         High-risk loans: 88%

# Summary

Although the accuracy score was very high, the dataset used to train the model was also very unbalanced, with over 30x the number of healthy loan data than risky loan data. Because of this, the model is better at predicting healthy loans than high-risk ones, seen in the disparity among precision, recall, and f1-scores. Though the model still did a fairly good job at predicting high-risk loans, a more balanced dataset would yield better results. Especially in this case, as predicting high-risk loans accurately is more important to a lending services company. I would recommend resampling the data to provide a more balanced dataset for the model. 
