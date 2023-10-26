# Restricted Boltzmann Machine (RBM) using PyTorch

This repository contains an implementation of a Restricted Boltzmann Machine (RBM) using PyTorch. The RBM is a generative stochastic artificial neural network that can learn a probability distribution over its set of inputs. In this project, we apply the RBM to collaborative filtering for movie recommendations using the MovieLens dataset.

## Table of Contents

- [Introduction](#introduction)
- [Dependencies](#dependencies)
- [Dataset](#dataset)
- [Data Preprocessing](#data-preprocessing)
- [RBM Architecture](#rbm-architecture)
- [Training the RBM](#training-the-rbm)
- [Testing the RBM](#testing-the-rbm)
- [Results](#results)
- [Usage](#usage)

## Introduction

The Restricted Boltzmann Machine is a powerful unsupervised learning algorithm that can discover underlying patterns in data. In this project, we use RBM to build a movie recommendation system. The RBM is trained on user ratings from the training dataset and can make personalized movie recommendations for users.

## Dependencies

To run this code, you need the following dependencies:

- Python 3.x
- PyTorch
- Pandas
- Numpy

## Dataset

We use the MovieLens dataset for this project. The dataset contains movie ratings by users. You can download the dataset using the provided links in the code.

## Data Preprocessing

The MovieLens dataset is preprocessed to prepare the training and test sets. The preprocessing steps include:

- Separating users, movies, and ratings.
- Converting the ratings to binary values (0 for not liked, 1 for liked).

## RBM Architecture

The RBM is implemented with the following architecture:

- Number of visible nodes (nv): Determined by the number of movies.
- Number of hidden nodes (nh): Set as 100 in this implementation.
- Weight matrix (W), visible bias (a), and hidden bias (b).

## Training the RBM

The RBM is trained using Contrastive Divergence (CD). The training steps include:

- Gibbs sampling for k steps.
- Updating weights and biases based on the difference between observed and reconstructed data.
- Calculating the training loss.

## Testing the RBM

The trained RBM is tested by comparing its predictions to the test set. The testing steps include:

- Using the RBM to predict user preferences.
- Comparing the predicted preferences to the test set.
- Calculating the test loss.

## Results

The RBM's performance is evaluated based on the test loss, which measures the accuracy of movie recommendations. With this metric, we obtained an Average Distance of 0.24, which is equivalent to about 75% of correct predictions. Hence, it works very well and has predictive power.

## Usage

You can run the RBM algorithm by following the steps outlined in the Jupyter notebook provided in this repository. It includes detailed comments and explanations for each section of the code.

---

Feel free to customize this README file to include more specific details about your implementation, such as hyperparameters used, additional features, and any other relevant information. This will help users understand and use your RBM implementation more effectively.
