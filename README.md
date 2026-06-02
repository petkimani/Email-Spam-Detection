# Email-Spam-Detection
A machine learning pipeline that classifies emails as spam or ham using TF-IDF vectorization and Logistic Regression

# Project overview
Spam emails remain a significant productivity drain and security risk. This project builds an end-to-end text classification system that takes raw email message text and predicts whether it is spam or legitimate (ham). The model is trained on a labeled SMS/email dataset and evaluated using standard classification metrics.

The approach converts raw text into numerical features using TF-IDF (Term Frequency–Inverse Document Frequency), then trains a Logistic Regression classifier — a fast, interpretable baseline well-suited for high-dimensional text problems.

train accuracy
98.71%
test accuracy
96.59%
model type
Logistic Reg.
features
TF-IDF

