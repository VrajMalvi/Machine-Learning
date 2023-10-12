# Model Selection using k-Fold Cross Validation and Grid Search

In this repository, you'll find code and explanations for model selection in machine learning using two essential techniques: **k-Fold Cross Validation** and **Grid Search**. The code is implemented in Jupyter Notebook (.ipynb) format and focuses on the problem of classifying a Social Network Ads dataset.

## Files in the Repository

1. **k_fold_cross_validation.ipynb**:
   - **Purpose**: This Jupyter Notebook demonstrates the use of k-Fold Cross Validation to evaluate the performance of a Support Vector Machine (SVM) model trained on the Social Network Ads dataset.
   - **Explanation**:
     - It starts with importing necessary libraries, loading the dataset, and performing data preprocessing (feature scaling).
     - The SVM model is trained with a radial basis function (RBF) kernel.
     - The code showcases how to apply k-Fold Cross Validation to estimate the model's performance using 10 folds, providing both mean accuracy and standard deviation.
     - The accuracy is visualized using decision boundaries in both the training and test sets.
   - **Outcome**: The model's performance is evaluated, showing an accuracy of around 90.33% with a standard deviation of 6.57%.

2. **grid_search.ipynb**:
   - **Purpose**: This Jupyter Notebook demonstrates the use of Grid Search to find the best hyperparameters for the SVM model on the same Social Network Ads dataset.
   - **Explanation**:
     - It begins with importing libraries, loading the dataset, and performing data preprocessing (feature scaling).
     - The SVM model is trained with a radial basis function (RBF) kernel.
     - Grid Search is applied to search for the best combination of hyperparameters (C and gamma) that maximize accuracy using 10-fold Cross Validation.
     - The best accuracy and the corresponding hyperparameters are reported.
     - The accuracy is visualized using decision boundaries in both the training and test sets.
   - **Outcome**: Grid Search identifies the best parameters, achieving a slightly improved accuracy of 90.67% with hyperparameters C=0.5 and gamma=0.6.

3. **Social Network Ads.csv**:
   - **Purpose**: This is the dataset used in both notebooks.
   - **Explanation**: The dataset contains information about users and whether they purchased a product. The goal is to predict whether a user will purchase the product based on their age and estimated salary.

## Why k-Fold Cross Validation and Grid Search?

- **k-Fold Cross Validation** is used to evaluate the model's performance robustly. It helps ensure that the model's performance estimates are not influenced by the specific data split, reducing the risk of overfitting.

- **Grid Search** is employed to find the best hyperparameters for the model. It systematically explores different combinations of hyperparameters and helps in fine-tuning the model for optimal performance.

These techniques are crucial for building reliable and well-performing machine learning models.

Feel free to explore the Jupyter Notebooks and adapt the code to your own datasets and machine learning projects. 
