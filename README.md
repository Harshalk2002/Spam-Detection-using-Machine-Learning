📧 Spam Detection using Machine Learning


📚 Overview
This project implements a Spam Detection system for classifying SMS messages as Spam or Ham (Not Spam) using Machine Learning techniques.
The models were trained and evaluated on the SMSSpamCollection dataset from the UCI Machine Learning Repository.
The primary goal is to filter out unwanted and fraudulent messages while maintaining a balance between Precision and Recall.

🗂️ Table of Contents
Overview
Dataset
Preprocessing
Exploratory Data Analysis
Models Implemented
Results
Challenges & Solutions
Conclusion
How to Run
Requirements

Dataset Name: SMSSpamCollection Dataset
Description:
Contains 5,574 English SMS messages labeled as either:
Spam: Unwanted promotional/fraudulent messages
Ham: Legitimate messages
Source: UCI Machine Learning Repository
🧹 Preprocessing
Converted all text to lowercase
Removed punctuation, numbers, and special characters
Removed extra spaces
Tokenization and TF-IDF Vectorization for feature extraction
Dataset split: 80% training, 20% testing
📊 Exploratory Data Analysis
Class Distribution:
Visualized the ratio of Spam vs. Ham messages
Message Length Distribution:
Spam messages are typically shorter
Common Spam Words:
"free", "win", "text", "claim", etc.
🤖 Models Implemented
Model	Description
Naïve Bayes	MultinomialNB, ideal for text classification tasks
Logistic Regression	Regularized Logistic Regression, with GridSearchCV for hyperparameter tuning
✅ Results
Naïve Bayes:
Accuracy: 96.86%
Precision: 100%
Recall: 76.51%
F1-Score: 86.69%
Logistic Regression:
Accuracy: 96.77%
Precision: 99.13%
Recall: 76.51%
F1-Score: 86.36%
Confusion Matrix Analysis:
Naïve Bayes achieved perfect precision, meaning no false positives
Logistic Regression delivered a better balance between precision and accuracy
⚖️ Model Comparison
Model	Pros	Cons
Naïve Bayes	Perfect Precision (100%)	Lower Recall (76.51%)
Logistic Regression	Balanced performance	Slightly lower Precision
➡️ Best Choice?

Use Naïve Bayes if avoiding false positives is critical
Use Logistic Regression for more balanced predictions
Future improvements: Ensemble models, deep learning approaches
🚧 Challenges & Solutions
Balancing Precision and Recall
➡️ Used different classifiers and hyperparameter tuning
Preprocessing Optimization
➡️ Switched from Count Vectorizer to TF-IDF for better results
Logistic Regression convergence issues
➡️ Increased max_iter to 500 to resolve warnings
🎯 Conclusion
Both models successfully detect spam messages with high accuracy.

Naïve Bayes provides zero false positives
Logistic Regression gives a balanced approach
Future work may explore ensemble methods and deep learning techniques for improved performance.


⚖️ License
This project is licensed under the MIT License.

⭐️ Acknowledgments
UCI Machine Learning Repository
scikit-learn and the Python open-source community
Matplotlib and Seaborn for visualization tools

