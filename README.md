Task 4 – Spam Detection with Naive Bayes + TF-IDF

This project implements a spam detection classifier using Naive Bayes and TF-IDF vectorization. The model is trained on the classic SMS Spam Collection Dataset.

✨ Features

Load & preprocess dataset (Ham = 0, Spam = 1)

Text preprocessing using TF-IDF Vectorization

Train a Multinomial Naive Bayes classifier

Evaluate model with:

Accuracy

Classification Report

Confusion Matrix Heatmap

Test with custom input messages

📂 Project Structure
task4_spam_detection/
│── spam_detection.py       # Main implementation
│── SMSSpamCollection       # Dataset (from UCI)
│── requirements.txt
│── README.md

⚙️ Setup & Run
1. Install requirements
pip install -r requirements.txt

2. Download dataset

Download from: SMS Spam Collection

Extract and place the file SMSSpamCollection in the project folder.

3. Run the script
python spam_detection.py

📊 Sample Output
Dataset Sample
  label                                             message
0   ham  Go until jurong point, crazy.. Available only ...
1   ham                      Ok lar... Joking wif u oni...
2  spam  Free entry in 2 a wkly comp to win FA Cup fina...

Model Evaluation
Accuracy: 0.97
Classification Report:
              precision    recall  f1-score   support
Ham              0.98       0.99      0.98      965
Spam             0.92       0.88      0.90      150

Confusion Matrix

(Visualized as heatmap)

Prediction Demo
Message: Congratulations! You have won free tickets. Claim now! --> Prediction: Spam
Message: Hey, what time is our meeting? --> Prediction: Ham
Message: URGENT! Your loan is overdue, pay immediately. --> Prediction: Spam

🔮 Future Improvements

Try other classifiers (Logistic Regression, SVM, Random Forest)

Use Word2Vec / GloVe embeddings

Build a Flask/Streamlit app for interactive spam checking
