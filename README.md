# Handwritten-Digits-Recognition-By-Random-Forest-and-Adaboost


Based on this repository document, here is a complete explanation of the Random Forest and AdaBoost classification process for the MNIST handwritten digit dataset.

## Summary
The document explores the application of two ensemble machine learning models, Random Forest and AdaBoost, to classify handwritten digits from the MNIST dataset. It demonstrates the complete process from data preparation to model training and evaluation. Both models achieve a high level of accuracy, showcasing the effectiveness of ensemble methods for this classification task. The document also includes an important note regarding the use of Support Vector Machines (SVMs) as the base estimator for AdaBoost.

## 1. Data Loading and Preparation
The process begins by importing the necessary libraries from scikit-learn (sklearn), pandas, numpy, and matplotlib. The MNIST handwritten digit dataset is then loaded. Each image in the dataset is an 8x8 pixel grid, which is then reshaped into a flattened array of 64 features to be used for model training. The corresponding labels for each digit are also prepared.


## 2. Random Forest Classification
A Random Forest classifier is used first. This is a model that builds an ensemble of decision trees and makes predictions based on the majority vote of the trees for a classification task. The model is initialized with 1000 estimators and is trained on the first 1000 data points. The model's performance is then evaluated on the remaining 797 data points. The document reports that this Random Forest model achieved a high accuracy of 93% on the test data.

## 3. AdaBoost Classification
The document then introduces the AdaBoost (Adaptive Boosting) classifier. This model uses a Support Vector Classifier (SVC) with an RBF kernel as its base estimator. The document highlights a crucial point: boosting algorithms typically work best with weak base models (like simple decision trees), and using a strong learner like an SVM can be slow and may lead to overfitting. Despite this, the AdaBoost model is trained and also achieves a high level of accuracy.

## Conclusion
The document effectively demonstrates the power of ensemble methods, specifically Random Forest and AdaBoost, for handwritten digit classification. Both models proved to be highly accurate on the MNIST dataset. The analysis highlights the importance of choosing the right algorithm for a task and understanding the implications of different hyperparameter and base estimator choices, such as the note about using strong learners like SVMs in boosting algorithms.




