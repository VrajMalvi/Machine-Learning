# Self-Organizing Map (SOM) for Fraud Detection

This project implements a Self-Organizing Map (SOM) for detecting potential fraud cases in a dataset. The SOM is an unsupervised machine learning technique used to cluster and detect patterns in complex data. In this specific application, the goal is to identify potential fraud cases rather than predicting a binary outcome (0 or 1).

## Table of Contents
- [Introduction](#introduction)
- [Dataset](#dataset)
- [Feature Scaling](#feature-scaling)
- [Training the SOM](#training-the-som)
- [Visualizing the Results](#visualizing-the-results)
- [Finding the Frauds](#finding-the-frauds)
- [Results](#results)

## Introduction

Self-Organizing Maps (SOM) are a type of artificial neural network that are particularly useful for visualizing and analyzing high-dimensional data. They can detect relationships, clusters, and anomalies in the data without requiring labeled examples. In this project, SOM is applied to detect potential fraudulent customers from a dataset of credit card applications.

## Dataset

The dataset used in this project contains information about credit card applications. Each entry in the dataset includes various features about the applicants and whether their applications were approved or not (0 for not approved and 1 for approved). The dataset also includes customer IDs to trace back to fraud cases.

## Feature Scaling

Before training the SOM, feature scaling is applied to the dataset. Feature scaling ensures that all input features have the same scale and prevents some features from dominating others.

## Training the SOM

A SOM is initialized with dimensions of 10x10, and the input data's dimensionality is set to 15. The SOM is trained with a radius of influence (sigma) and a learning rate to adapt to the input data. Training is carried out over 100 iterations.

## Visualizing the Results

The SOM's training results are visualized using a heatmap. Each node in the SOM is represented by a color, showing how strongly it is associated with the input data.

## Finding the Frauds

After training the SOM, specific grid nodes are identified that strongly represent potential fraud cases. The code maps data points to these nodes, and the fraud cases are concatenated and stored in the `frauds` variable. These cases are then inverse-transformed to their original scale.

## Results

The detected fraud cases include the customer IDs, which can be further investigated for potential fraudulent activities.

This project showcases the power of SOM in unsupervised learning for anomaly detection and can be used to identify suspicious cases that merit closer examination.

To run this project, you'll need Python, the `MiniSom` package, and the dataset of credit card applications. The complete code is available in this repository.

[Original Dataset](Credit_Card_Applications.csv)

For more details, check out the Python code files and feel free to experiment with your data.
