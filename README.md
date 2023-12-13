# MNIST Handwritten Digits Classifier

## Project Overview
This project aims to build and optimize models for classifying handwritten digits (0-9) from the MNIST dataset. The focus is on developing several classifiers, including Gaussian classifiers with identity and common covariance, logistic regression classifiers, and their regularized versions. The project specifically emphasizes distinguishing between digits 2 and 3, and also extends to a multi-class classifier for all digits.

## Component 1: Gaussian Classifiers for Digits 2 and 3
- **Objective**: To differentiate between handwritten digits 2 and 3 from the MNIST dataset.
- **Methods**: 
  - Data Subset: Selected only digits 2 and 3 from the MNIST dataset for targeted classification.
  - Gaussian Classifier with Identity and Common Covariance: Developed classifiers considering different covariance structures.
  - Logistic Regression Classifier: Implemented to classify between the two digits.
  - Regularization Techniques: Applied to enhance model performance and prevent overfitting.
- **Optimization**: 
  - Dimensionality Reduction: Utilized eigenvalue decomposition.
  - Regularization in Logistic Regression: Addressed overfitting issues.
  - Hyperparameter Tuning: Conducted to identify optimal regularization strength.

## Component 2: Multiclass Classification for All Digits
- **Objective**: To classify each of the 10 digits (0-9) in the MNIST dataset.
- **Methods**:
  - Standard Scaling and PCA: Employed for effective feature extraction.
  - Gaussian Multi-Channel Classifier with Covariance: Developed for handling multiple classes.
  - Multiclass Logistic Regression: Implemented both regularized and non-regularized versions.
- **Optimization**:
  - PCA: Used for reducing dimensions while retaining significant variance.
  - Regularized Logistic Regression: Improved model's generalization capabilities.
  - Hyperparameter Tuning: Performed to optimize the model based on validation set performance.

## Implementation Details
- **Libraries Used**: The project utilizes NumPy for numerical operations, Matplotlib for visualization, SciPy for scientific computations, and scikit-learn for machine learning algorithms.
- **Data Preprocessing**:
  - Scaling: Employed StandardScaler to normalize features.
  - PCA: Applied to reduce data dimensions, maintaining 95% of the variance.
- **Model Evaluation**:
  - Data Splitting: Divided the dataset into training, validation, and test sets for a comprehensive evaluation.
  - Metrics: Focused on accuracy and the count of misclassifications as key performance indicators.

## Challenges and Solutions
- **Overfitting with High-dimensional Data**: Overcoming overfitting was a challenge, especially with high-dimensional data. This was addressed by implementing regularization in logistic regression models and using PCA for dimensionality reduction.
- **Bias-Variance Tradeoff**: Managing the bias-variance tradeoff was crucial. Systematic hyperparameter tuning and cross-validation were key strategies employed to achieve this balance.

## Conclusion
This project illustrates the application of various machine learning models to classify handwritten digits from the MNIST dataset. Emphasis on optimization and regularization underscores their significance in practical machine learning scenarios. The project demonstrates that with thoughtful preprocessing and model tuning, high accuracy in digit classification is achievable.
