# Project Repository Overview

## Introduction to the Repository
This repository hosts a diverse collection of machine learning projects, including classifiers for handwritten digits and a NeRF (Neural Radiance Fields) implementation. The primary focus is on applying and optimizing various models to solve distinct problems, from digit recognition using the MNIST dataset to creating 3D scene representations with NeRF techniques.

## Project 1: MNIST Handwritten Digits Classification

### Overview
The goal is to classify handwritten digits (0-9) using the MNIST dataset. We explore Gaussian classifiers, logistic regression, and their regularized forms, emphasizing binary classification (digits 2 and 3) and extending to multiclass classification for all digits.

### Component 1: Binary Classification of Digits 2 and 3
- **Objective**: Distinguish between digits 2 and 3.
- **Approach**:
  - Data Subset Selection, Gaussian Classifiers with varied covariance structures, Logistic Regression, and Regularization to mitigate overfitting.
- **Optimization**:
  - Eigenvalue-based Dimensionality Reduction, Regularization in Logistic Regression, and Hyperparameter Tuning.

### Component 2: Multiclass Classification for Digits 0-9
- **Objective**: Classify all ten digits.
- **Approach**:
  - Feature extraction via Standard Scaling and PCA, Gaussian Multi-Channel Classifier, and Multiclass Logistic Regression.
- **Optimization**:
  - Dimension reduction with PCA, Regularized Logistic Regression, and Hyperparameter Adjustments.

### Implementation and Evaluation
- **Tools**: NumPy, Matplotlib, SciPy, scikit-learn.
- **Data Handling**: StandardScaler for normalization, PCA for dimensionality reduction.
- **Metrics**: Accuracy and misclassification count.

### Challenges
Addressing overfitting in high-dimensional data and managing the bias-variance tradeoff through regularization and systematic tuning.

### Conclusion
The project demonstrates the efficacy of machine learning models in digit classification, highlighting the importance of optimization and regularization.

## Project 2: Neural Radiance Fields (NeRF) Implementation

### Overview
An exploration into NeRF, utilizing PyTorch for constructing a 3D scene representation by synthesizing novel views from sparse input images.

### Core Components
- Positional Encoding for input coordinates.
- Sequential fully-connected layers for modeling volume density and color.
- Rendering rays for image synthesis with transmittance and volume rendering techniques.

### Implementation Details
- **Libraries**: PyTorch, NumPy, Matplotlib, DataLoader for batch processing.
- **Training**: Loss computation, backpropagation, and epoch-wise training with visualization of results.
- **Optimization**: Adam optimizer, learning rate scheduling.

### Challenges and Solutions
Effective 3D scene representation requires precise modeling of light transport and geometry, addressed through meticulous network design and training strategies.

### Conclusion
This project showcases the application of NeRF in creating photorealistic 3D scenes, emphasizing the potential of deep learning in computer vision and graphics.

---
