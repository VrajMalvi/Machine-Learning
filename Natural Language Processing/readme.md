# Natural Language Processing with Sentiment Analysis

This repository contains Python code to perform Natural Language Processing (NLP) with sentiment analysis on a dataset of restaurant reviews. The code demonstrates the preprocessing steps, creating a Bag of Words model, and training two different classification models: Naive Bayes and Logistic Regression.

## Table of Contents

- [Introduction](#introduction)
- [Prerequisites](#prerequisites)
- [Usage](#usage)
- [Results](#results)
- [License](#license)

## Introduction

In this project, we analyze a dataset of restaurant reviews to classify them as positive or negative based on the sentiments expressed in the text. The following steps are performed:

1. **Importing the libraries**: We import the necessary Python libraries, including NumPy, Matplotlib, and pandas.

2. **Importing the dataset**: The dataset containing restaurant reviews is loaded from a CSV file (`Restaurant_Reviews.tsv`) using pandas.

3. **Cleaning the texts**: We preprocess the text data by removing special characters, converting text to lowercase, removing stopwords, and applying stemming to reduce words to their root form.

4. **Creating the Bag of Words model**: We create a Bag of Words (BoW) model using the CountVectorizer from scikit-learn. This step involves tokenizing the text and building a vocabulary of unique words.

5. **Splitting the dataset**: We split the dataset into a training set and a test set for model evaluation.

6. **Training the Naive Bayes model**: We use a Gaussian Naive Bayes classifier to train a sentiment analysis model on the training set.

7. **Predicting the Test set results**: We make predictions on the test set using the trained Naive Bayes model and evaluate its performance.

8. **Training the Logistic Regression model**: We repeat the process by training a sentiment analysis model using Logistic Regression.

9. **Predicting the Test set results**: We make predictions on the test set using the trained Logistic Regression model and evaluate its performance.

## Prerequisites

Before running the code, make sure you have the following dependencies installed:

- Python (3.x)
- NumPy
- Matplotlib
- pandas
- NLTK (Natural Language Toolkit)
- scikit-learn

You can install the required libraries using the following command:

\`\`\`bash
pip install numpy matplotlib pandas nltk scikit-learn
\`\`\`

\`\`\`markdown
# Usage

Clone this repository to your local machine:

\`\`\`bash
git clone https://github.com/your-username/natural-language-processing.git
\`\`\`

Navigate to the project directory:

\`\`\`bash
cd natural-language-processing
\`\`\`

Execute the Jupyter Notebook or Python script to run the code. You can use a code editor or a Jupyter Notebook to open the provided .ipynb or .py file.

# Results

The code provided in this repository demonstrates the process of performing sentiment analysis on restaurant reviews using both a Naive Bayes classifier and a Logistic Regression classifier. The results obtained are as follows:

**Naive Bayes Classifier:**

Confusion Matrix:

\`\`\`lua
[[55 42]
 [12 91]]
\`\`\`

Accuracy: 0.73

**Logistic Regression Classifier:**

Confusion Matrix:

\`\`\`lua
[[80 17]
 [28 75]]
\`\`\`

Accuracy: 0.775

These results provide an understanding of the effectiveness of the two models in classifying restaurant reviews based on sentiment.

# License

This project is licensed under the MIT License - see the LICENSE file for details.

\`\`\`csharp
\`\`\`
\`\`\`
