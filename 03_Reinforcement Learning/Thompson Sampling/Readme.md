# Thompson Sampling

This repository contains the implementation of the Thompson Sampling algorithm for solving the multi-armed bandit problem. In this context, the algorithm is applied to optimize the selection of advertisements (ads) in an advertising campaign.

## Table of Contents

- [Introduction](#introduction)
- [Implementation](#implementation)
- [Usage](#usage)
- [Results](#results)

## Introduction

Thompson Sampling is a popular algorithm for making sequential decisions in an uncertain environment, where the goal is to balance exploration (trying different options) and exploitation (selecting the best-known option) to maximize cumulative rewards. In this implementation, we use Thompson Sampling to select the most effective ad to display to users.

## Implementation

### Libraries Used
- `numpy` and `random` for mathematical and randomization operations.
- `matplotlib.pyplot` for visualizing the results.
- `pandas` for reading and managing the dataset.

### Dataset
The dataset (`Ads_CTR_Optimisation.csv`) contains historical data on user interactions with different ads. It is used to simulate the selection of ads and observe the rewards.

### Thompson Sampling Algorithm
The implementation of the Thompson Sampling algorithm is provided in the Python script. The key steps include:
- Initializing parameters and variables, such as the number of arms (ads) and success/failure counts for each arm.
- Sampling from the posterior distribution for each arm (Beta distribution with parameters based on success and failure counts).
- Selecting the arm with the highest sampled value (representing the arm with the highest estimated success probability).
- Simulating the reward for the selected arm based on the dataset.
- Updating success and failure counts and accumulating the total reward.

## Usage

To use this implementation, follow these steps:
1. Ensure you have Python installed on your system.
2. Clone this repository to your local machine.
3. Place the dataset file (`Ads_CTR_Optimisation.csv`) in the same directory as the Python script.
4. Run the Python script to execute the Thompson Sampling algorithm.

## Results

The results of the Thompson Sampling algorithm are visualized using a histogram, showing the number of times each ad was selected over the simulation rounds. This visualization helps identify the ad that was selected most frequently, indicating the optimal choice for maximizing rewards.

