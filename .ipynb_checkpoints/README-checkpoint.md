# credit-risk-classification
Explain the purpose of the analysis.

- The purpose of the analysis is to train and evaluate the model for the loan risk.

Explain what financial information the data was on, and what you needed to predict.

- The dataset includes loan_size, interest_rate, borrower_income, debt_to_income, num_of_accounts, dergatory_marks, total_debt and load_status. Based on the availabe data, we need to predict the accuracy of load_status of 0 = healthy loan and 1 = risky loan for each loan.

Provide basic information about the variables you were trying to predict (e.g., value_counts).

- The dataset includes 75036 healthy loans and 2500 risky loans.

Describe the stages of the machine learning process you went through as part of this analysis.

- split the dataset into train and test
- create and predict logistic regression model with the original data
- create and predict logistic regression model with the sampled training data

Briefly touch on any methods you used (e.g., LogisticRegression, or any resampling method).

- We used logisticregression method to predict the outcomes from dataset starting with cleaning the data and splitting it into test and train subset, then use labeled data to train the model and then validate the data to test how well the model is able to predict labels, and lastly predict labels for unclassified data.

# Results

Using bulleted lists, describe the balanced accuracy scores and the precision and recall scores of all machine learning models.

Machine Learning Model 1: Description of Model 1 Accuracy, Precision, and Recall scores.

- 99% of the data are correctly predicted compared to the total number of observations.
- 100% of the healthy loans that classified by the modal as heathy loans were actuallly heathy loans while 85% of the risky loans were actually risky
- 99% of all the actual healthy loan samples, all were correctly classified as heathy while 91% of the risky loan were correctly classified as risky.

Machine Learning Model 2: Description of Model 2 Accuracy, Precision, and Recall scores.

- 99% of the data are correctly predicted compared to the total number of observations.
- 99% of the healthy loans that classified by the modal as heathy loan were actuallly heathy loan while 99% of the risky loan were actually risky
- 99% of all the actual healthy loan samples, all were correctly classified as heathy while 99% of the risky loan were correctly classified as risky.

# Summary

- The result from the logistic regression model with the resampled training data using RandomOverSampler function performs better based on the 99% accuracry, precision, and recall classification report for both healthy '0' and risky '1' loan status. Logistic regression model with orginal data is also good, but it was a bit less accurate compared to the resampled training data. Since the purpose of this analysis is to evaluate the model for the loan risk, both '1' and '0' are equally important for prediction.