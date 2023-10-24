# Stock Price Prediction with Recurrent Neural Network (RNN)

This project demonstrates the use of Recurrent Neural Networks (RNNs) to predict stock prices, specifically focusing on Google's stock prices in this example.

## Overview

Stock price prediction is a common application of RNNs in the field of time series forecasting. The goal is to use historical stock price data to predict future prices. In this project, we use a specific type of RNN known as Long Short-Term Memory (LSTM) to make these predictions.

## Procedure

### Data Preprocessing

1. **Importing the Data**: We start by importing the training data from the 'Google_Stock_Price_Train.csv' file.

2. **Feature Scaling**: We use Min-Max scaling to normalize the stock price data to a range between 0 and 1.

3. **Creating Sequences**: We create sequences of stock prices with 60 time steps in the past and use them to predict the next price. This involves organizing the data into input sequences (X) and output labels (y).

### Building and Training the RNN

4. **Building the RNN**: We construct an LSTM-based RNN model with multiple layers. The `return_sequences` parameter is set to `True` for intermediate layers to capture the sequence of hidden states.

5. **Compiling and Training**: The model is compiled with an optimizer (e.g., Adam) and a loss function (mean squared error). We fit the model to the training data over multiple epochs.

### Making Predictions

6. **Getting Real Stock Prices**: We import the test data for January 2017 ('Google_Stock_Price_Test.csv') to obtain the real stock prices.

7. **Predicting Stock Prices**: To predict January data, we need the previous 60 days' data. We concatenate the training and test data and reshape it. We then use the trained model to predict stock prices for January.

### Visualizing the Results

8. **Visualizing Predictions**: We use Matplotlib to visualize the predicted and real stock prices for January 2017. The results are shown in a line chart.

## Model Evaluation

For regression problems like stock price prediction, we typically use metrics such as Root Mean Squared Error (RMSE) to evaluate the model's performance. However, in this project, we are more interested in the direction of the predictions rather than their absolute values.

We want to check if our predictions follow the same directions as the real stock prices.

## Getting Started

To run this code, you need Python with libraries like NumPy, Pandas, Matplotlib, and Keras installed. The training and test datasets should be provided in CSV format.



