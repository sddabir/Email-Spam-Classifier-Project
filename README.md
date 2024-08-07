# Email-Spam-Classifier-Project

# Overview

This project aims to build a spam classifier using machine learning techniques. The goal is to accurately classify emails as either spam or ham (non-spam). We'll use the Apache SpamAssassin's public datasets to train and test our classifier.

# Steps to Reproduce


Download and Prepare Data: Downloaded examples of spam and ham from Apache SpamAssassin's public datasets. Unzipped the datasets and got familiarized with the data format.

Data Splitting: Split the datasets into a training set and a test set. This ensures that our model is evaluated on unseen data, helping to assess its generalization performance.

Data Preparation Pipeline: Wrote a data preparation pipeline to convert each email into a feature vector. The pipeline will transform emails into sparse vectors indicating the presence or absence of each possible word. Various preprocessing steps such as stripping off email headers, converting text to lowercase, removing punctuation, replacing URLs and numbers, and performing stemming may be applied.

Model Training and Evaluation: Trained different classifiers using the prepared data and evaluate their performance. Experimented with various models such as Logistic Regression, Random Forest, Support Vector Machine (SVM), etc.

Fine-tuning: Fine-tuned the selected model(s) by adjusting hyperparameters to optimize performance. Used grid search or randomized search techniques for hyperparameter tuning.

Model Evaluation: Evaluated the final model(s) using appropriate evaluation metrics such as accuracy, precision, recall, and F1-score. Pid close attention to both precision (the ratio of correctly predicted spam emails to the total predicted spam emails) and recall (the ratio of correctly predicted spam emails to the total actual spam emails) to ensure a balanced performance.


# Results

Logistic Regression Model: After training and evaluation, the logistic regression model achieved a mean cross-validation score of 0.9858. It exhibited high precision and recall of 96.88% and 97.89%, respectively, indicating excellent performance in both correctly identifying spam emails and minimizing false positives.


# Libraries used

Python 3.x

NumPy

Pandas

Scikit-learn

Beautiful Soup (for HTML parsing)

Others as needed
