Spam Filter

Overview

This project implements a spam filter using a combination of Naive Bayes and Random Forest models. The dataset for this project was manually created by labeling every message as either "spam" or "ham" (not spam) based on a personal mailbox. The dataset includes several features: username, email domain, subject, and text body.

Data

The dataset contains the following features:

Username: The username of the email account.
Email Domain: The domain part of the email address.
Subject: The subject line of the email.
Text Body: The content of the email message.
The data was manually labeled as spam or ham to create a balanced dataset for training and evaluation.

Methodology

Text Body Processing
The text body of the emails was processed using simple tokenization and vectorization techniques:

Tokenization: Splitting the text into individual words.
Vectorization: Converting text into numerical vectors suitable for model input.
Model Training
Naive Bayes Model:
Used to classify the text body of emails.
It focuses on the content of the email to determine if it is spam or not.
Random Forest Model:
Utilized to process other features: username, email domain, and subject.
Trains on these features to contribute to the overall classification.
Model Integration
The Naive Bayes and Random Forest models were combined into a Logistic Regression model. This integrated approach allowed for the fusion of text-based and feature-based predictions to achieve a robust classification system.

Results

Total Accuracy: 98%
Confusion Matrix: Evaluated to check for overfitting, especially considering the class imbalance.
Confusion Matrix
The confusion matrix was analyzed to ensure that the model generalizes well despite the imbalance between spam and ham classes.
