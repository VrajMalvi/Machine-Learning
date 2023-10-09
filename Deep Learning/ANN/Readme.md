# Artificial Neural Network for Customer Churn Prediction

## Problem Statement

The bank has been experiencing an unusually high churn rate, with a significant number of customers leaving the bank. To address this issue and reduce customer churn, we have access to a dataset containing information about 10,000 customers over a six-month period, including whether or not they left the bank during that time. Our goal is to develop a predictive model that can identify customers at a higher risk of leaving the bank. By doing so, the bank can take proactive measures to retain these customers and reduce the churn rate.

## Solution Overview

### Data Preprocessing

We start by importing the necessary libraries for data preprocessing and model building. We then load the dataset, selecting relevant features and labels. The data is preprocessed as follows:

- **Label Encoding**: The "Gender" column is label-encoded to convert gender values (e.g., "Male" and "Female") into numerical format.

- **One-Hot Encoding**: The "Geography" column is one-hot encoded to convert country names (e.g., "France," "Spain," "Germany") into binary columns.

- **Data Splitting**: The dataset is split into training and testing sets to train and evaluate the model's performance.

- **Feature Scaling**: Feature scaling is applied to standardize numerical features, ensuring they have similar scales.

### Building the Artificial Neural Network (ANN)

We construct an Artificial Neural Network (ANN) for predictive modeling. The network architecture consists of:

- **Input Layer**: Input features are fed into the neural network.

- **Hidden Layers**: Two hidden layers with ReLU activation functions are added.

- **Output Layer**: The output layer uses a sigmoid activation function to provide predictions.

### Model Training

The ANN is compiled with the Adam optimizer and binary cross-entropy loss function. We train the model on the training dataset, specifying the number of epochs and batch size for optimization.

### Making Predictions

We use the trained ANN to make predictions, including single observations and test set results.

## Usage

To use this code:

Clone this repository to your local machine:

```bash
git https://github.com/VrajMalvi/Machine-Learning/tree/main/ANN
```


- **True Positives (TP)**: 219
- **True Negatives (TN)**: 1487
- **False Positives (FP)**: 108
- **False Negatives (FN)**: 186

### Accuracy Score

The accuracy score is a critical measure of the model's overall performance. It indicates the percentage of correct predictions out of all predictions made by the model.

In our case, the accuracy score is approximately __85.3%__. This means that our model correctly predicts customer churn with an accuracy of __85.3%__, which is considered a good performance metric.

The combination of the confusion matrix and accuracy score provides a comprehensive assessment of our model's ability to identify and retain at-risk customers.

These metrics are essential for evaluating the effectiveness of our customer churn prediction model and making informed decisions to reduce churn and improve customer retention.
