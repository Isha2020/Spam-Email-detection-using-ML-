Spam Email Classifier
This is a simple Spam Email Classifier Web App built using Python, Streamlit, and Scikit-learn.

It predicts whether a message is SPAM or HAM (not spam) using a Naive Bayes machine learning model.

🚀 Features
Simple and interactive web interface

Real-time prediction of spam or ham messages

Built with machine learning using a real email dataset

🛠️ Built With
Python

Streamlit – for building the web app

Scikit-learn – for machine learning

Pandas – for data handling

📂 Dataset
The app uses a JSON file email-text-data.json that contains:

MESSAGE: the email or message text

CATEGORY: the label (spam or ham)

📋 Example:
json
Copy
Edit
[
  {
    "MESSAGE": "Congratulations! You've won a $1000 gift card. Click here.",
    "CATEGORY": "spam"
  },
  {
    "MESSAGE": "Let's have a meeting at 10 am tomorrow.",
    "CATEGORY": "ham"
  }
]
⚙️ How It Works
The dataset is loaded and the text is converted into numerical form using CountVectorizer.

A Naive Bayes classifier is trained to detect patterns typical of spam messages.

The user inputs a message into the app.

The trained model predicts whether the message is SPAM or HAM and displays the result in real time.

▶️ How to Run the App
Clone this repository:

bash
Copy
Edit
git clone https://github.com/your-username/spam-email-classifier.git
cd spam-email-classifier
Install the required libraries:

bash
Copy
Edit
pip install -r requirements.txt
Run the app:

bash
Copy
Edit
streamlit run app.py
Open in your browser (automatically opens at):
http://localhost:8501

📦 File Structure
bash
Copy
Edit
spam-email-classifier/
├── app.py                  # Main Streamlit app file
├── email-text-data.json    # Dataset containing email messages and labels
├── requirements.txt        # Required Python libraries
└── README.md               # Project description and documentation
📌 Example Prediction
User input:

sql
Copy
Edit
Congratulations! Claim your free prize now.
Model output:

nginx
Copy
Edit
SPAM ❌
🧠 About the Algorithm and Model
This application uses the Multinomial Naive Bayes algorithm — a fast and efficient text classification model — to detect spam messages.

🔍 What is Multinomial Naive Bayes?
Naive Bayes is a family of probabilistic algorithms based on Bayes’ Theorem. It assumes that the features (words in this case) are independent of each other.

Multinomial Naive Bayes is particularly suited for text classification tasks where features represent word frequency.

It’s widely used in spam detection due to its simplicity and accuracy.

🧪 Model Training Process
The dataset is loaded from email-text-data.json containing email texts and their labels (spam or ham).

Text Preprocessing:

Text is converted into numerical form using CountVectorizer.

Common English stop words like "the", "is", "in" are removed.

The data is split:

70% for training

30% for testing

The Multinomial Naive Bayes model is trained on the training data and then used to predict new inputs.

📊 Key Libraries and Tools Used
scikit-learn:

CountVectorizer: For converting text into numerical data

MultinomialNB: Naive Bayes classifier

train_test_split: To split data into training and testing sets

pandas: For loading and processing the dataset

streamlit: For creating the web interface

📬 Future Improvements
Add support for more languages

Include message length and sender metadata as features

Use advanced NLP techniques like TF-IDF or word embeddings

Deploy the model online (e.g., Streamlit Cloud or Heroku)
