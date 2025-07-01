# Spam-Email-detection-using-ML-
web-based Spam Email Classifier built with Python, Streamlit, and Scikit-learn that detects whether a message is spam or not using a trained Naive Bayes model and NLP techniques.
This project is a Spam Email Detection Web App built using Python, Streamlit, and Scikit-learn. It predicts whether an email message is spam or ham (not spam) using a Multinomial Naive Bayes model.

The model is trained on a labeled email dataset. Each message is preprocessed using Natural Language Processing (NLP) techniques and then vectorized using CountVectorizer to convert text into numerical features.

🚀 Features

Simple and interactive web interface

Real-time prediction of spam or ham messages

Trained using actual email data

Built with efficient machine learning techniques


🛠️ Technologies Used

Python – programming logic and ML pipeline

Streamlit – for building the web app interface

Scikit-learn – ML model and text preprocessing

Pandas – data handling and analysis


📂 Dataset

The dataset used is a JSON file (email-text-data.json) that includes:

MESSAGE: The email/message text

CATEGORY: Label (spam or ham)


⚙️ How It Works

1. The text data is cleaned and transformed into vectors using CountVectorizer.


2. A Multinomial Naive Bayes classifier is trained on the dataset.


3. The user enters a message into the Streamlit app.


4. The model predicts and displays whether it is spam or ham.
5. 
