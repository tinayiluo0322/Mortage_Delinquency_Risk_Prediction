# Predicting Mortgage Delinquency Risk

## Project Description

This project aims to build a predictive model to assess the likelihood of mortgage delinquency, specifically whether a homeowner will be at least 30 days late on a mortgage payment during the first two years of the mortgage. The goal is to help a mortgage servicing firm differentiate between high-risk and low-risk mortgages to make informed purchasing decisions.

## Objectives

- Develop a predictive model for mortgage delinquency.
- Use real data from Freddie Mac to train and validate the model.
- Ensure the model's predictions meet the stakeholder's requirement of maintaining a delinquency rate of purchased mortgages below 5%.

## Dataset

### Data Source

The dataset used in this project is from Freddie Mac, covering all US Standard single-family home mortgages purchased or insured in a single calendar year, along with payment data from that year and the subsequent two years.

- **Source:** [Freddie Mac Single-Family Loan-Level Dataset](https://www.freddiemac.com/research/datasets/sf-loanlevel-dataset)

### Data Description

The dataset includes various features related to the mortgage, borrower, and property, such as:
- Loan amount
- Interest rate
- Loan-to-value ratio
- Borrower credit score
- Debt-to-income ratio
- Property type and location
- Payment history

## Methodology

### Data Preprocessing

1. **Data Cleaning:** Handle missing values, outliers, and inconsistent data entries.
2. **Feature Engineering:** Create new features that might be relevant for predicting mortgage delinquency, such as payment patterns and borrower demographics.
3. **Data Splitting:** Split the data into training and testing sets to evaluate the model's performance.

### Model Development

1. **Model Selection:** gradient boosting calssifier.
2. **Hyperparameter Tuning:** Use techniques such as grid search and cross-validation to find the optimal hyperparameters for the chosen model.
3. **Model Training:** Train the model on the training dataset using the selected algorithm and optimized hyperparameters.

### Model Evaluation

1. **Performance Metrics:** Evaluate the model using metrics such as accuracy, precision, recall, F1 score, and AUC-ROC.
2. **False Omission Rate (FOR):** Calculate the FOR to measure the proportion of negative predictions that were incorrect.
3. **Threshold Selection:** Choose an appropriate decision threshold to balance the trade-off between false positives and false negatives.

## Results

### Model Performance

The final model was evaluated based on its ability to predict mortgage delinquency within the first two years. Key performance metrics include:

- **Accuracy:** Measure of overall correctness of the model.
- **Precision:** Proportion of positive predictions that were correct.
- **Recall:** Proportion of actual positives that were correctly identified.
- **F1 Score:** Harmonic mean of precision and recall.
- **AUC-ROC:** Area under the Receiver Operating Characteristic curve, indicating the model's discriminatory ability.

### False Omission Rate (FOR)

The model's False Omission Rate (FOR) was calculated to be around 4.90%, indicating the proportion of negative predictions that were incorrect. This meets the stakeholder's requirement of maintaining a delinquency rate of purchased mortgages below 5%.

## Conclusion

The predictive model developed in this project provides reliable assessments of mortgage delinquency risk. With a False Omission Rate of 4.90%, the model meets the stakeholder's requirement of keeping the delinquency rate of purchased mortgages below 5%. Therefore, the model is capable of providing the level of performance needed to help the mortgage servicing firm make informed purchasing decisions.
