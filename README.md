# Fake_news_Detection

📌 Project Summary: Fake News Detection Using Machine Learning & NLP

This project focuses on building a machine learning model to automatically detect whether a news article is real or fake using natural language processing (NLP) techniques.

1. 🔍 Dataset Loading & Preprocessing

Loaded a labeled dataset of news articles containing:

text – the content of the news

label – 0 (real) or 1 (fake)

Dropped unnecessary columns such as:

id, author, title

Checked for missing values and removed NA rows.

2. 🧹 Text Cleaning Using NLP

Created a custom clean_text() function to prepare text for modeling:

Converted text to lowercase

Removed punctuation, numbers, and special characters using regex

Removed stopwords

Used PorterStemmer for word stemming

Final cleaned text stored in a new column: cleaned_text

3. 📊 Exploratory Data Analysis (EDA)

Used Seaborn countplot to visualize distribution of fake vs real news.

Generated WordClouds for:

Fake news

Real news
This helped visualize commonly used words in each category.

4. 🧠 Feature Extraction

Converted text data into numerical vectors using:

TF-IDF Vectorizer

Set max_features = 3000

Created:

x → TF-IDF features

y → labels

Performed train-test split (80% training, 20% testing).

5. 🤖 Model Building & Training

Trained multiple machine learning algorithms:

Naive Bayes

GaussianNB

MultinomialNB

BernoulliNB
Evaluated accuracy for each.

Other ML Models

Used several advanced algorithms:

Logistic Regression

SVM (Sigmoid kernel)

K-Nearest Neighbors

Decision Tree

Random Forest

Extra Trees Classifier

Gradient Boosting

XGBoost

A custom function computed and compared accuracies for all models.

6. 🏆 Model Evaluation

Calculated accuracy for each classifier.

Compared performance of all algorithms.
(Usually, MultinomialNB, SVM, and XGBoost perform best for text classification.)

7. 🧪 Testing on New Samples

Tested the final trained models on custom real/fake news text samples.
Predictions were made using:

BernoulliNB

XGBoost
