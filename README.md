# Phishing

📧 Phishing Email Detection Using Machine Learning

A machine learning–based system designed to detect and classify phishing emails, including AI-generated and human-written threats.
The model is trained using real-world datasets such as Ling-Spam, Enron Emai, and Preprocessed trec, and uses NLP techniques to analyze email content for malicious patterns.

**🚀 Features**

-> Detects phishing vs. non-phishing emails using ML classification
-> Supports AI-generated and human-crafted phishing detection
-> Uses TF-IDF vectorization + Logistic Regression
-> Real-world datasets (Ling-Spam, Enron Emai, and Preprocessed trec)
-> Gmail IMAP integration to read real-time incoming emails
-> Automatically:
  --> Clean and preprocess email data
  --> Predict phishing probability
  --> (Optional) Export results to CSV
  --> (Optional) Move phishing emails to spam

**🧠 Machine Learning Workflow**

1. Dataset Collection
-> PhishTank
-> Enron Email Dataset
-> SpamAssassin Corpus

2. Preprocessing
-> HTML tag removal
-> URL, email, and special character cleaning
-> Stopword removal
-> Lowercasing

3. Feature Extraction
-> TF-IDF Vectorization

4. Model Training
-> Logistic Regression (best performance)
-> Evaluation: Accuracy, F1-score, Precision, Recall

5. Model Saving
-> phishing_model.pkl
-> tfidf_vectorizer.pkl

6. Pipeline Building
-> Combined into a single phishing_pipeline.pkl

**📥 Real-Time Email Scanning**

This project supports Gmail IMAP to fetch emails automatically.
Capabilities:
-> Reads new emails from inbox
-> Extracts subject + body
-> Runs model prediction
-> Outputs phishing probability
-> (Optional) Saves results to CSV
-> (Optional) Automatically move phishing emails to SPAM
