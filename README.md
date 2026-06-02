# Email-Spam-Detection
A machine learning pipeline that classifies emails as spam or ham using TF-IDF vectorization and Logistic Regression

# Project overview
Spam emails remain a significant productivity drain and security risk. This project builds an end-to-end text classification system that takes raw email message text and predicts whether it is spam or legitimate (ham). The model is trained on a labeled SMS/email dataset and evaluated using standard classification metrics.

The approach converts raw text into numerical features using TF-IDF (Term Frequency–Inverse Document Frequency), then trains a Logistic Regression classifier — a fast, interpretable baseline well-suited for high-dimensional text problems.

#Model training
1. TF-IDF vectorization
Raw text cannot be fed directly into a mathematical model. TF-IDF converts each message into a sparse numeric vector where each dimension represents a unique word in the vocabulary. The score balances word frequency within a document against how common it is across all documents — giving higher weight to distinctive, meaningful words.

2. Logistic Regression models the log-odds of a message being ham (1) vs spam (0) as a linear combination of TF-IDF features. Despite its simplicity, it performs exceptionally well on text classification because the high-dimensional TF-IDF space is often linearly separable.

# Confusion matrix interpretation — the model is tuned conservatively. It rarely blocks legitimate email (only ~1.2% false alarm rate) but misses roughly 1 in 6 spam messages. That's the right trade-off for most use cases, since a missed newsletter is far less damaging than a blocked job offer.
