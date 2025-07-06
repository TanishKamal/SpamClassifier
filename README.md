Project Overview
This project uses a dataset of SMS messages labeled as "ham" or "spam" to train a text classification model. It includes preprocessing, feature extraction, visualization, and model evaluation. The final model can predict whether a new message is spam or not.

Features

Data preprocessing & cleaning
Text transformation using stemming, tokenization, and stopword removal
Feature extraction using TF-IDF
Model training with various Naive Bayes classifiers
Model evaluation using accuracy, confusion matrix, and precision
Exploratory Data Analysis (EDA) and visualizations

Dataset

The dataset used is spam.csv, containing labeled SMS messages:
ham: Non-spam messages
spam: Unwanted promotional messages

Tech Stack

Python
NumPy, Pandas
Matplotlib, Seaborn (for data visualization)
NLTK (Natural Language Toolkit) for NLP
Scikit-learn for model building and evaluation

Workflow

1. Data Cleaning
Removed unwanted columns
Renamed and relabeled target column
Removed duplicate entries

2. EDA (Exploratory Data Analysis)
Message length analysis
Word and sentence token analysis
Histogram and pairplot visualizations

3. Text Preprocessing
Applied a custom transformation pipeline:
Lowercasing
Tokenization
Removing non-alphanumeric characters
Removing stopwords and punctuation
Stemming using PorterStemmer

4. Feature Extraction
Used TF-IDF Vectorizer with max_features=3000 for converting text to numerical vectors.

5. Model Building
Tried three types of Naive Bayes classifiers:
GaussianNB
MultinomialNB (best performer)
BernoulliNB

6. Model Evaluation
MultinomialNB gave:
Accuracy: ~97%
Precision: 1.0

Sample Visuals
Pie chart showing spam/ham distribution
Histogram of message lengths
Pairplot for numerical features (words, characters, sentences)
