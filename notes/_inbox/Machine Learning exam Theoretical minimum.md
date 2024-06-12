---
aliases: 
publish: true
created: 2024-06-08 13:05
parent:
  - "[[Machine Learning MOC]]"
connected:
  - "[[Machine Learning exam questions-answers]]"
---

#### 1. Supervised learning problem statement
> [!question]- Supervised Learning Problem Statement
TARGET DECK: Math::Machine Learning TM
START
Math_ONE_side
TITLE: Supervised Learning Problem Statement
DESCRIPTION: 
A supervised learning problem involves learning a function from labeled training data to make predictions on unseen data. The goal is to map input data (features) to output labels (targets) using a model that generalizes well to new data.
FORMULA: 
Given a dataset $\{(x_i, y_i)\}_{i=1}^n$, the objective is to find a function $f$ such that $f(x) \approx y$ for new data points $(x, y)$.
ADDITIONAL:
Examples include regression (predicting continuous values) and classification (predicting discrete labels). In regression, $y$ is continuous, while in classification, $y$ is categorical. 
PICTURE:
ID: 1717834200728
END

> [!question]- Types of Supervised Learning
TARGET DECK: Math::Machine Learning TM
START
Math_ONE_side
TITLE: Types of Supervised Learning
DESCRIPTION: 
Supervised learning can be divided into two main categories: regression and classification. 
ADDITIONAL:
- Regression: Predicting a continuous output (e.g., predicting house prices).
- Classification: Predicting a discrete label (e.g., classifying emails as spam or not spam).
PICTURE:
ID: 1717834200732
END

> [!question]- Key Components in Supervised Learning
TARGET DECK: Math::Machine Learning TM
START
Math_ONE_side
TITLE: Key Components in Supervised Learning
DESCRIPTION: 
The key components of a supervised learning problem are the input features, the output labels, and the model that maps inputs to outputs. 
ADDITIONAL:
- Input Features: Represent the data points (e.g., height, weight).
- Output Labels: The target values to predict (e.g., price, category).
- Model: The algorithm used to learn from the input-output pairs (e.g., linear regression, decision trees).
PICTURE:
ID: 1717834200734
END


1. Unsupervised learning problem statement. Provide at least two example problems.
#### 2. Unsupervised learning problem statement. Provide at least two example problems.



#### 3. What is i.i.d. data?
#### 4. How does a Naive Bayesian Classifier work? Why is it naive?
#### 5. Linear regression model for MSE minimization problem. Write down the formula and the derivative of the loss function w.r.t. weights.
#### 6. Write down a gradient descent step. How to adjust it for huge datasets?
#### 7. What is the likelihood? Where is Maximum Likelihood Estimation (MLE) usually used?
#### 8. What is cross-validation? How does the number of folds affect the validation?
#### 9. What is overfitting and underfitting? How to detect them?
#### 10. What is the difference between parameters and hyperparameters? Provide an example for linear models/decision trees.
#### 11. What is a regularization? What is the difference between L1 and L2 regularization in linear models? Is it the only way to constrain the solution?
#### 12. Does L2 regularization regularize the bias term (w_0 or b)? Why?
#### 13. Why is it a good idea to normalize data before applying a linear model?
#### 14. Provide a linear classification problem statement. What is a margin?
#### 15. What are precision and recall? How to use them to measure the model quality?
#### 16. Assume the dataset for binary classification is imbalanced, so 95% of data belong to the first class. How to adjust the classification quality measures, to work with such data? Why?
#### 17. What is ROC AUC? How to build the ROC curve?
#### 18. Logistic loss function. How is it related to Maximum likelihood estimation?
#### 19. Support Vector Machine main idea. The optimization functional for linearly separable case.
#### 20. Describe the greedy optimization algorithm for the decision tree.
#### 21. Why can an unconstrained decision tree achieve zero error on the training set with unique objects?
#### 22. How to assign a class label for the object in the tree leaf in classification?
#### 23. How to assign a class label for the object in the tree leaf in regression? Does it depend on the information criterion?
#### 24. What is bagging?
#### 25. What is Random Forest? How does it differ from Bagging over decision trees?
#### 26. How are base algorithms being trained in gradient boosting?
#### 27. How does backpropagation work in neural networks? What will be vector by vector derivative?
#### 28. How does the Convolutional layer work? What is the convolution operation?
#### 29. Why fully connected (dense) networks are not the best choice to work with image data? Why do CNNs perform better?
#### 30. How does basic RNN (Vanilla RNN) work?
#### 31. How does dropout work?
#### 32. How do dropout and batch normalization change their behaviour on the inference stage?
#### 33. What is the problem statement for the Principal Component Analysis?