# Wine Quality Prediction with Ensemble Learning

## Overview

This repository contains Python code for predicting the quality of red wines using ensemble learning methods. The implemented models include Decision Tree Classifier, Bagging Classifier, and Random Forest Classifier. The code also involves hyperparameter tuning using GridSearchCV to optimize the Random Forest Classifier.

## Dataset

### Description

The dataset consists of various attributes of red wine samples, including fixed acidity, volatile acidity, citric acid, residual sugar, chlorides, free sulfur dioxide, total sulfur dioxide, density, pH, sulphates, alcohol, and quality. The 'quality' column represents the target variable, categorizing wines into different quality levels.

## Ensemble Learning Methods

### Decision Tree Classifier

- A standalone decision tree classifier is implemented.
- Decision trees make predictions based on recursive binary splits of the feature space.

### Bagging Classifier

- Bagging (Bootstrap Aggregating) is applied to a base decision tree classifier.
- Multiple decision trees are trained on bootstrapped samples of the dataset.
- Predictions are made by averaging or voting.

### Random Forest Classifier

- Random Forest is an ensemble method that builds multiple decision trees and merges them together.
- Each tree is trained on a random subset of features and bootstrapped samples.
- Predictions are made by averaging or voting.

## Hyperparameter Tuning

- GridSearchCV is used to perform hyperparameter tuning for the Random Forest Classifier.
- Hyperparameters like 'n_estimators' and 'max_depth' are optimized to improve model performance.

## Conclusion

The ensemble learning methods, particularly Bagging and Random Forest, show improved predictive performance compared to a standalone Decision Tree Classifier. 

