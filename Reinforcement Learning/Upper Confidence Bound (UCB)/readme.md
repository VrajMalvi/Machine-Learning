# Upper Confidence Bound (UCB) Algorithm

This GitHub repository contains a Python implementation of the Upper Confidence Bound (UCB) algorithm. UCB is a popular algorithm for solving the multi-armed bandit problem, where an agent needs to make decisions about which arms (actions) to pull to maximize cumulative rewards while balancing exploration and exploitation.

## Code Overview

### 1. Importing the Libraries

The code starts by importing the necessary Python libraries, including NumPy for numerical operations, Matplotlib for data visualization, and Pandas for data handling.

### 2. Importing the Dataset

It loads the dataset ('Ads_CTR_Optimisation.csv') using Pandas. The dataset likely contains information about rewards (click-through rates) for different ads.

### 3. Implementing UCB

The core of the UCB algorithm is implemented in this section. Here's a breakdown of the key components:

- `N` and `d` represent the number of users (or rounds) and the number of ads (arms), respectively.
- `ads_selected` keeps track of the ads selected at each round.
- `numbers_of_selections` records the number of times each ad has been selected.
- `sums_of_rewards` stores the cumulative rewards obtained for each ad.
- `total_reward` keeps track of the total reward accumulated.

The code iterates through each round (from 0 to `N`) and selects the ad with the highest upper confidence bound. It calculates the UCB for each ad based on the observed rewards and the number of selections.

### 4. Visualizing the Results

After running the UCB algorithm, the code visualizes the results by creating a histogram of ad selections. This histogram shows how many times each ad was selected throughout the experiment.

## How to Use

To use this UCB algorithm, you can follow these steps:

1. Ensure you have Python installed, along with the required libraries (NumPy, Matplotlib, and Pandas).

2. Download the 'Ads_CTR_Optimisation.csv' dataset or replace it with your own dataset if needed.

3. Run the Python code, and it will execute the UCB algorithm on the provided dataset.

4. The results will be visualized with a histogram, showing the distribution of ad selections.

## Contributions

If you have any improvements, bug fixes, or additional features to suggest for this UCB implementation, feel free to open an issue or submit a pull request. Contributions are welcome and encouraged!


Happy bandit solving!
