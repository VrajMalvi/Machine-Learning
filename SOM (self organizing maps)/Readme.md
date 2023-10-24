# Mega Case Study - Hybrid Deep Learning Model for Fraud Detection

This project combines Self-Organizing Maps (SOM) and Artificial Neural Networks (ANN) to create a hybrid deep learning model for fraud detection. The goal is to identify potential fraud cases in a dataset.

## Table of Contents
- [Introduction](#introduction)
- [Part 1 - SOM](#part-1---som)
  - [Importing Libraries](#importing-libraries)
  - [Importing the Dataset](#importing-the-dataset)
  - [Feature Scaling](#feature-scaling)
  - [Training the SOM](#training-the-som)
  - [Visualizing the Results](#visualizing-the-results)
  - [Finding the Frauds](#finding-the-frauds)
- [Part 2 - Going from Unsupervised to Supervised Deep Learning](#part-2---going-from-unsupervised-to-supervised-deep-learning)
  - [Creating Matrix of Features](#creating-matrix-of-features)
  - [Creating Dependent Variable](#creating-dependent-variable)
- [Part 3 - ANN](#part-3---ann)
  - [Feature Scaling](#feature-scaling-ann)
  - [Building the ANN](#building-the-ann)
  - [Training the ANN](#training-the-ann)
  - [Predicting Test Set Results](#predicting-test-set-results)

## Introduction

This project combines unsupervised SOM to cluster and detect potential fraud patterns and supervised ANN to classify fraud cases. By employing this hybrid approach, it becomes possible to identify suspicious activities within a dataset.

## Part 1 - SOM

### Importing Libraries

In this section, we import necessary libraries and prepare the environment for the SOM and ANN implementation.

### Importing the Dataset

The dataset used in this project contains information about credit card applications. The goal is to identify fraudulent applications from this dataset.

### Feature Scaling

Feature scaling is applied to standardize the input data for training the SOM, ensuring that all features have the same scale.

### Training the SOM

A SOM of dimensions 10x10 is trained with input data, including parameters for radius of influence and learning rate. Training is carried out over 100 iterations.

### Visualizing the Results

The results of SOM training are visualized with a heatmap, where each node represents a different association with input data.

### Finding the Frauds

The trained SOM is used to identify potential fraud cases by mapping data points to specific grid nodes and concatenating the identified cases.

## Part 2 - Going from Unsupervised to Supervised Deep Learning

### Creating Matrix of Features

The matrix of features for training the ANN is created by removing unnecessary columns.

### Creating Dependent Variable

The dependent variable is created to classify applicants as potential fraud cases based on the SOM's findings.

## Part 3 - ANN

### Feature Scaling (ANN)

The features are scaled for the ANN as well to ensure consistency in data representation.

### Building the ANN

The ANN model is constructed using TensorFlow with one input layer, one hidden layer with ReLU activation, and one output layer with sigmoid activation.

### Training the ANN

The ANN is trained on the dataset using the Adam optimizer and binary cross-entropy loss. The model is trained over 10 epochs.

### Predicting Test Set Results

The ANN predicts test set results, which include customer IDs and the likelihood of fraud. The results are sorted based on the likelihood of fraud.

This hybrid deep learning model combines the strengths of SOM for unsupervised clustering and ANN for supervised classification to identify potential fraud cases. You can experiment with this code and dataset to apply this approach to your specific needs.

To run this project, ensure you have Python and TensorFlow installed. The complete code is available in this repository.

For more details, check out the Python code files and the complete dataset, and feel free to adapt the code for your own projects.

[Original Dataset](Credit_Card_Applications.csv)
