# XGBoost Classifier for Tumor Classification

This repository contains Python code for training an XGBoost classifier to classify tumor samples into benign (0) and malignant (1) based on a dataset.

## Overview

In this project, we use the XGBoost algorithm to build a classification model for tumor detection. The dataset contains information about tumors, with labels 2 and 4, which represent benign and malignant tumors. We convert these labels to 0 for benign and 1 for malignant to prepare the data for classification.

## Code Structure

The code is organized as follows:

- **Importing the Required Libraries:** We start by importing the necessary Python libraries, including NumPy, Matplotlib, and pandas.

- **Loading the Dataset:** We load the tumor dataset from a CSV file (`Data.csv`) using pandas. The dataset contains features (X) and tumor labels (y).

- **Data Preprocessing:** We convert the original tumor labels (2 and 4) to binary labels (0 and 1) using NumPy's `np.where` function and create a new array `y_` to store the converted labels.

- **Splitting the Dataset:** We split the dataset into training and testing sets using `train_test_split` from scikit-learn.

- **Training the XGBoost Classifier:** We create an XGBoost classifier and train it on the training data.

- **Model Evaluation:** We evaluate the model by calculating the confusion matrix and accuracy on the test set.

- **k-Fold Cross-Validation:** We apply k-fold cross-validation to assess the model's performance more comprehensively.

## Results

- The confusion matrix for the model is as follows:

```lua
[[85 2]
[ 1 49]]
```


- The accuracy of the model on the test set is approximately 97.81%.

- k-Fold Cross-Validation shows an average accuracy of 96.71% with a standard deviation of 2.28%.

## Usage

You can use this code as a template for classifying tumors as benign or malignant in your own dataset. Simply replace the `Data.csv` file with your dataset and modify the code accordingly.

## Dependencies

- Python 3
- NumPy
- Matplotlib
- pandas
- scikit-learn
- XGBoost


Feel free to use, modify, and distribute this code for your projects.

For more details, you can refer to the [XGBoost documentation](https://xgboost.readthedocs.io/).
