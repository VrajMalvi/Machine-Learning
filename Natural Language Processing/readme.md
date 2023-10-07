# Sentiment Analysis with Natural Language Processing (NLP) in Python

Welcome to the Sentiment Analysis project! This repository demonstrates how to leverage the power of NLP to analyze customer reviews and determine their sentiment (positive or negative). Let's dive into the details:

## Project Overview

In this project, we tackle one of the most exciting challenges in NLP: sentiment analysis. We aim to classify restaurant reviews as either positive or negative based on their textual content. Understanding sentiment is crucial for businesses to gauge customer satisfaction and make data-driven decisions.

## Code Walkthrough

### 1. Importing the Libraries

We start by importing essential Python libraries:
- NumPy for numerical operations.
- Matplotlib for data visualization.
- Pandas for data manipulation.

### 2. Importing the Dataset

We load the restaurant reviews dataset, stored in a TSV (Tab-Separated Values) file. The dataset contains customer reviews and their associated sentiments.

### 3. Cleaning the Texts

This is where the magic begins! We meticulously clean the text data:
- Remove special characters, punctuation, and numbers.
- Convert text to lowercase for uniformity.
- Tokenize text into words.
- Remove common "stop words" (e.g., 'the', 'a', 'an') that don't provide valuable information.
- Apply stemming to reduce words to their root form (e.g., 'running' to 'run').

### 4. Creating the Bag of Words Model

We create a Bag of Words (BoW) model using scikit-learn's CountVectorizer. The BoW model represents each review as a vector of word frequencies. We carefully select the top 1500 most important words, discarding less informative ones.

### 5. Splitting the Dataset

To evaluate our model, we split the dataset into two parts:
- Training set: Used to train the machine learning model.
- Test set: Used to assess the model's performance on unseen data.

### 6. Training the Naive Bayes Model

We train a Naive Bayes classifier (specifically, GaussianNB) on the training set. Naive Bayes is a powerful algorithm for text classification tasks like sentiment analysis.

### 7. Predicting the Test Set Results

We put our trained model to the test! It predicts sentiments (positive or negative) for reviews in the test set.

### 8. Making the Confusion Matrix

We create a confusion matrix to dig deeper into the model's performance. It helps us understand true positives, true negatives, false positives, and false negatives.

### 9. Accuracy Score

The accuracy score provides a quantitative measure of our model's performance. It indicates the proportion of correctly classified reviews in the test set.

## Explore and Experiment

Feel free to explore the code, experiment with different datasets, or fine-tune the model for your specific NLP tasks. Sentiment analysis is just the beginning; NLP has a vast range of applications, from chatbots to language translation.

Happy coding and analyzing! 🍔📊😄
