# Supervised Learning – Discrete Variable Prediction: Fraud Detection

## Overview
This project focuses on employing machine learning algorithms to detect fraudulent credit card transactions. With fraudsters becoming increasingly sophisticated, traditional detection methods often fall short. Our approach leverages data science to build predictive models that can effectively identify fraudulent activities.

## Model Selection
We evaluate several classification algorithms to determine whether a transaction is fraudulent or legitimate:

- Logistic Regression
- Support Vector Machine (SVM)
- K-Nearest Neighbors (KNN)
- Decision Tree
- Random Forest
- Naive Bayes

## Dataset
The dataset utilized is a simulated credit card transaction dataset, encompassing both legitimate and fraudulent transactions from January 1, 2019, to December 31, 2020. It features various attributes, including transaction date, credit card number, merchant, transaction amount, and a binary fraud indicator.

### Dataset Features
- **Unnamed: 0**: Row index
- **trans_date_trans_time**: Transaction timestamp
- **cc_num**: Credit card number (masked/encrypted)
- **merchant**: Merchant identifier
- **category**: Transaction category
- **amt**: Transaction amount
- **first, last**: Cardholder's name
- **gender**: Cardholder's gender
- **street, city, state, zip**: Cardholder's address
- **lat, long**: Cardholder's geographical coordinates
- **city_pop**: Population of the city
- **job**: Cardholder's occupation
- **dob**: Date of birth
- **trans_num**: Transaction number
- **unix_time**: Transaction time in Unix format
- **merch_lat, merch_long**: Merchant's geographical coordinates
- **is_fraud**: Fraud indicator (0 = legitimate, 1 = fraudulent)

## Data Imbalance
The dataset is highly imbalanced, with approximately 99.42% of transactions being non-fraudulent (Class 0) and only 0.58% being fraudulent (Class 1). To address this imbalance, we will employ techniques such as SMOTE (Synthetic Minority Over-sampling Technique).

## Methodology
1. **Data Preprocessing**
   - **Feature Engineering**: Extract time features (hour, day of the week) and create new features for transaction frequency over the last 1, 7, and 30 days.
   - **Imbalance Handling**: Implement SMOTE to ensure balanced class representation during model training.

2. **Exploratory Data Analysis (EDA)**
   - Uncover patterns in the data, including transaction trends and feature correlations.

3. **Model Training and Evaluation**
   - Train models on the training set (80% of data) and evaluate on the test set (20%).
   - Use metrics such as accuracy, precision, recall, F1 score, AUC, and confusion matrix for evaluation.

4. **Pipeline Implementation**
   - Create a scikit-learn pipeline to streamline the preprocessing, training, and evaluation processes.

## Results
The Random Forest Classifier achieved the highest accuracy of **99.60%**, with precision at **0.91** and recall at **0.35**. SVM and KNN also performed well, albeit with slightly lower accuracy. The F1 score for Random Forest was **0.51**, indicating a trade-off between precision and recall.

### Handwritten Digits Prediction (Extra Credit)
As an additional task, we explored predicting handwritten digits using non-deep learning models, applying dimensionality reduction techniques like PCA and t-SNE to tackle high-dimensional image data challenges.

## Conclusion
This project showcases the application of various machine learning models for fraud detection in credit card transactions. By leveraging data preprocessing, feature engineering, and thorough model evaluation, we aim to enhance the accuracy of fraud detection systems, ultimately reducing financial losses for businesses and organizations. 
