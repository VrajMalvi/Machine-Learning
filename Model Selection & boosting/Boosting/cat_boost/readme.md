# CatBoost Classifier for Tumor Detection

This code demonstrates the use of CatBoost, a machine learning library, to classify tumor samples into benign (0) or malignant (1) based on a given dataset.

## Prerequisites

Make sure you have the following libraries installed in your Python environment:

- [CatBoost](https://catboost.ai/)
- [NumPy](https://numpy.org/)
- [Matplotlib](https://matplotlib.org/)
- [Pandas](https://pandas.pydata.org/)
- [Scikit-learn](https://scikit-learn.org/)

You can install CatBoost by running the following command:

```python
!pip install catboost
```

## Dataset
The dataset used in this code is loaded from a CSV file, `Data.csv`. It contains information about tumor samples and their corresponding classes (2 for benign, 4 for malignant).

## Data Preprocessing
The code loads the dataset, separates the features into `X` and the classes into `y`.

The classes (2 and 4) are mapped to (0 and 1) to indicate benign and malignant, respectively.

## Model Training
A CatBoostClassifier is used to train a machine learning model. It is a gradient boosting library that performs well on classification tasks without extensive hyperparameter tuning.

## Model Evaluation
The code evaluates the trained model using a test set and computes a confusion matrix and accuracy score to assess its performance.

It also performs k-fold cross-validation to estimate the model's accuracy and standard deviation.

# Running the Code
You can run this code in a Jupyter Notebook or any Python environment that has the required libraries installed. Ensure that the `Data.csv` file is in the same directory as this code.

# Results
The model achieves an accuracy of approximately 97.81% on the test set.

The k-fold cross-validation results in an average accuracy of 97.26% with a standard deviation of 2.03%.

This code demonstrates the use of CatBoost for tumor classification and serves as a template for similar classification tasks.

Feel free to adapt and extend the code for your specific use case.
