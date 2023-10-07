# Natural Language Processing (NLP) with Python

This repository contains code for performing Natural Language Processing (NLP) tasks using Python. In this project, we focus on sentiment analysis of restaurant reviews. Here's a breakdown of the code:

## Steps:

1. **Importing the Libraries**: We start by importing essential libraries, including NumPy, Matplotlib, and Pandas, for data manipulation and visualization.

2. **Importing the Dataset**: We load the restaurant reviews dataset from a TSV (Tab-Separated Values) file using Pandas. The dataset contains customer reviews and their corresponding sentiments (positive or negative).

3. **Cleaning the Texts**: In this crucial step, we preprocess the text data. The cleaning process involves removing special characters, converting text to lowercase, splitting text into words, removing stopwords, and applying stemming. This step prepares the text for analysis.

4. **Creating the Bag of Words Model**: We create a Bag of Words (BoW) model using scikit-learn's CountVectorizer. The BoW model tokenizes the text data, builds a vocabulary of words, and represents each review as a vector of word frequencies. We limit the number of features to 1500, which means we consider the 1500 most important words.

5. **Splitting the Dataset**: The dataset is split into training and test sets using scikit-learn's `train_test_split` function. This division allows us to evaluate the model's performance on unseen data.

6. **Training the Naive Bayes Model**: We train a Naive Bayes classifier (GaussianNB) on the training set. The Naive Bayes algorithm is a popular choice for text classification tasks like sentiment analysis.

7. **Predicting the Test Set Results**: The trained model is used to make predictions on the test set, allowing us to assess its accuracy in classifying reviews.

8. **Making the Confusion Matrix**: A confusion matrix is generated to evaluate the model's performance further. It helps us understand how well the model classifies positive and negative reviews.

9. **Accuracy Score**: The accuracy score of the model on the test set is calculated, providing an overall measure of its performance.

Feel free to explore the code and dataset to gain insights into sentiment analysis using NLP techniques. If you have any questions or suggestions, please don't hesitate to reach out. Happy coding! 😄📊🍔🍕
