# AutoEncoders

## Overview

This project implements an AutoEncoder-based recommendation system using PyTorch. AutoEncoders are used to model user preferences in a movie recommendation dataset. The goal is to build a model that can predict which movies a user might like based on their previous ratings.

## Dataset

The MovieLens 100K dataset is used in this project. The dataset contains user ratings for movies, and it's divided into training and test sets.

## Code Structure

- `Downloading the Dataset`: The code includes downloading and unzipping the MovieLens dataset.

- `Importing the Libraries`: This section imports the necessary Python libraries, including NumPy, pandas, and PyTorch.

- `Preparing the Training Set and Test Set`: The training and test sets are loaded from the dataset files. The data is preprocessed and organized for further use.

- `Creating the Architecture of the Neural Network`: An AutoEncoder architecture is defined using PyTorch's `nn.Module`. It consists of several fully connected layers for encoding and decoding user preferences.

- `Training the SAE`: The AutoEncoder model is trained using the training set. Mean Squared Error (MSE) is used as the loss function, and RMSprop is used as the optimizer.

- `Testing the SAE`: The trained AutoEncoder is tested on the test set, and the test loss is calculated.

## How to Run

To run this code, make sure you have Python, PyTorch, NumPy, and pandas installed. Execute each section of the code sequentially, following the provided comments.

## Results

The project's main result is the test loss, which is indicative of how well the AutoEncoder can predict user preferences. In this example, the test loss is approximately 0.9605.

Feel free to experiment with the architecture and hyperparameters to improve the recommendation system's accuracy.
