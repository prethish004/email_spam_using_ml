# email_spam_using_ml
# 📧 Spam Detection using Machine Learning

This project is focused on detecting spam messages in SMS text data using various machine learning models. It includes training, evaluation, sample testing, and a Streamlit app for real-time predictions.

## 📁 Dataset

- **Source**: [`SMSSpamCollection`](https://archive.ics.uci.edu/ml/datasets/sms+spam+collection)
- **Description**: A collection of 5,572 SMS messages labeled as either spam or ham (not spam).
- **Format**: Tab-separated text with two columns: `label` and `message`.

## 🧹 Preprocessing

- Converted `label` values:  
  - `'ham'` → `0`  
  - `'spam'` → `1`
- Split into **training** and **test** sets (80/20).
- Vectorization using:
  - **Bag of Words (BoW)** via `CountVectorizer`
  - **TF-IDF** via `TfidfVectorizer`

## 🧠 Machine Learning Models

Trained and evaluated the following models:

1. **Logistic Regression**
2. **K-Nearest Neighbors (KNN)**
3. **Support Vector Machine (SVM)**
4. **Random Forest**
5. **Naive Bayes**
6. **Decision Tree**

Each model was trained on both **BoW** and **TF-IDF** features and evaluated using:

- Accuracy
- Precision
- Recall
- F1 Score
- Confusion Matrix

## 🔍 Sample Predictions

Tested models on new messages like:

- `"Free entry in 2 a weekly competition to win tickets!"`
- `"Hey, are we still on for dinner tonight?"`
- `"URGENT! Your Mobile No. has won £2000!"`

Models predicted if the messages were `Spam` or `Ham`.

## 🧪 Evaluation Example 
![image](https://github.com/user-attachments/assets/5df2343f-3b35-4dfa-917d-10aa6ccae5ac)

![image](https://github.com/user-attachments/assets/7636052a-804c-4daf-abdf-8a57698c24a6)
![image](https://github.com/user-attachments/assets/4e57f4a8-71fc-4547-9e0e-8f8db8f69d25)
![image](https://github.com/user-attachments/assets/83ec4e52-870b-44c3-b33a-f50c8beb78b1)

