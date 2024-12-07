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

> [!question]- Unsupervised Learning Problem Statement
TARGET DECK: Math::Machine Learning TM
START
Math_TWO_side
TITLE: Unsupervised Learning Problem Statement
DESCRIPTION:
Unsupervised learning involves training a model using data that does not have labeled responses. The goal is to infer the natural structure present within a set of data points.
FORMULA: 
N/A
ADDITIONAL:
Examples include:
1. **Clustering**: Grouping a set of objects in such a way that objects in the same group are more similar to each other than to those in other groups.
   - Example: Customer segmentation in marketing where customers are grouped based on purchasing behavior.
2. **Dimensionality Reduction**: Reducing the number of random variables under consideration by obtaining a set of principal variables.
   - Example: Principal Component Analysis (PCA) used in image compression.
PICTURE:
ID: 1718373874778
END


#### 3. What is i.i.d. data?
> [!question]- i.i.d. Data Definition
TARGET DECK: Math::Machine Learning TM
START
Math_TWO_side
TITLE: i.i.d. Data
DESCRIPTION:
i.i.d. stands for independent and identically distributed. This term is used to describe a set of random variables that are both independent from each other and follow the same probability distribution.
FORMULA:
N/A
ADDITIONAL:
- **Independent**: Each data point does not provide any information about any other data point.
- **Identically Distributed**: Each data point is drawn from the same probability distribution.
Example: In a coin toss experiment, each toss is i.i.d. because the outcome of one toss does not affect the outcome of another, and each toss has the same probability distribution (50% heads, 50% tails).
PICTURE:
ID: 1718373927853
END

> [!question]- Importance of i.i.d. Assumption
TARGET DECK: Math::Machine Learning TM
START
Math_ONE_side
TITLE: Importance of i.i.d. Assumption
DESCRIPTION:
The i.i.d. assumption is critical in many machine learning algorithms and statistical methods because it simplifies the mathematical models and ensures the validity of various theoretical results.
FORMULA:
N/A
ADDITIONAL:
- Simplifies the calculation of probabilities and expectations.
- Ensures that the law of large numbers and central limit theorem can be applied.
- Essential for the performance guarantees of many algorithms, such as those based on empirical risk minimization.
Example: In linear regression, assuming that the error terms are i.i.d. allows us to derive properties of the ordinary least squares estimators.
PICTURE:
ID: 1718373927856
END

#### 4. How does a Naive Bayesian Classifier work? Why is it naive?

> [!question]- Naive Bayesian Classifier
TARGET DECK: Math::Machine Learning TM
START
Math_TWO_side
TITLE: Naive Bayesian Classifier
DESCRIPTION: 
A Naive Bayesian Classifier works by calculating the posterior probability of each class given the input features, and the class with the highest posterior probability is chosen as the predicted class. It uses Bayes' theorem to compute the posterior probability:
FORMULA: 
$P(C_k | \mathbf{x}) = \frac{P(\mathbf{x} | C_k) P(C_k)}{P(\mathbf{x})}$
ADDITIONAL:
Here, $P(C_k | \mathbf{x})$ is the posterior probability of class $C_k$ given the feature vector $\mathbf{x}$, $P(\mathbf{x} | C_k)$ is the likelihood of $\mathbf{x}$ given class $C_k$, $P(C_k)$ is the prior probability of class $C_k$, and $P(\mathbf{x})$ is the evidence or the total probability of the feature vector $\mathbf{x}$. The classifier is considered "naive" because it assumes that all features are independent given the class label, which is rarely true in real-world data.
PICTURE:
ID: 1718374085227
END

> [!question]- Why Naive Bayesian Classifier is  naive?
TARGET DECK: Math::Machine Learning TM
START
Math_ONE_side
TITLE: Why Naive Bayesian Classifier is  naive?
DESCRIPTION: 
The Naive Bayesian classifier is termed "naive" because it assumes that all the features are mutually independent given the class label. This assumption simplifies the computation of the likelihood $P(\mathbf{x} | C_k)$ as the product of the individual likelihoods of the features:
FORMULA: 
$P(\mathbf{x} | C_k) = \prod_{i=1}^{n} P(x_i | C_k)$
ADDITIONAL:
Despite this strong assumption, the Naive Bayesian classifier often performs surprisingly well in practice, especially for text classification tasks such as spam detection and sentiment analysis.
PICTURE:
ID: 1718374085230
END


#### 5. Linear regression model for MSE minimization problem. Write down the formula and the derivative of the loss function w.r.t. weights.

> [!question]- Mean Squared Error (MSE) Formula
TARGET DECK: Math::Machine Learning TM
START
Math_ONE_side
TITLE: Mean Squared Error (MSE) Formula
DESCRIPTION: 
The Mean Squared Error (MSE) is a common loss function in linear regression that measures the average of the squares of the errors.
FORMULA: 
$L(\mathbf{w}) = \frac{1}{n} \sum_{i=1}^n (y_i - \mathbf{x}_i^\top \mathbf{w})^2$
ADDITIONAL:
Where $n$ is the number of samples, $y_i$ is the true value, $\mathbf{x}_i$ is the feature vector for the $i$-th sample, and $\mathbf{w}$ is the weight vector.
PICTURE:
ID: 1718374196829
END

> [!question]- Gradient of the Loss Function w.r.t. Weights
TARGET DECK: Math::Machine Learning TM
START
Math_ONE_side
TITLE: Gradient of the Loss Function w.r.t. Weights
DESCRIPTION: 
The gradient of the MSE loss function with respect to the weights is used to update the weights in gradient descent.
FORMULA: 
$\nabla L(\mathbf{w}) = -\frac{2}{n} \mathbf{X}^\top (\mathbf{y} - \mathbf{X}\mathbf{w})$
ADDITIONAL:
Where $\mathbf{X}$ is the matrix of input features, $\mathbf{y}$ is the vector of true values, and $\mathbf{w}$ is the vector of weights.
PICTURE:
ID: 1718374196832
END



#### 6. Write down a gradient descent step. How to adjust it for huge datasets?
> [!question]- Gradient Descent Step
TARGET DECK: Math::Machine Learning TM
START
Math_ONE_side
TITLE: Gradient Descent Step
DESCRIPTION: 
Gradient descent is an optimization algorithm used to minimize the loss function by iteratively updating the weights in the opposite direction of the gradient of the loss function.
FORMULA: 
$\mathbf{w} := \mathbf{w} - \alpha \nabla L(\mathbf{w})$
ADDITIONAL:
Where $\alpha$ is the learning rate and $\nabla L(\mathbf{w}) = -\frac{2}{n} \mathbf{X}^\top (\mathbf{y} - \mathbf{X}\mathbf{w})$ is the gradient of the loss function with respect to the weights. This approach is computationally expensive for large datasets.
PICTURE:
ID: 1718374256603
END

> [!question]- Adjusting Gradient Descent for Huge Datasets
TARGET DECK: Math::Machine Learning TM
START
Math_ONE_side
TITLE: Adjusting Gradient Descent for Huge Datasets
DESCRIPTION: 
For huge datasets, Stochastic Gradient Descent (SGD) or Mini-batch Gradient Descent is used to update weights more efficiently by using a subset of data.
FORMULA: 
$\mathbf{w} := \mathbf{w} - \alpha \nabla L_i(\mathbf{w})$
ADDITIONAL:
In SGD, the gradient is computed for each sample $i$. In Mini-batch Gradient Descent, the gradient is computed for a batch of samples. Both methods reduce computational cost and can converge faster.
Example of Mini-batch Gradient Descent:
$\mathbf{w} := \mathbf{w} - \alpha \frac{1}{m} \sum_{j=1}^{m} \nabla L_j(\mathbf{w})$
where $m$ is the batch size.
PICTURE:
ID: 1718374256607
END


#### 7. What is the likelihood? Where is Maximum Likelihood Estimation (MLE) usually used?
> [!question]- Likelihood
TARGET DECK: Math::Machine Learning TM
START
Math_ONE_side
TITLE: Likelihood
DESCRIPTION: 
In statistics, likelihood is a function of the parameters of a statistical model given data. It represents the probability of the observed data under different parameter values.
FORMULA: 
$L(\theta; \mathbf{X}) = P(\mathbf{X}|\theta)$
ADDITIONAL:
Likelihood is used to estimate the parameters of a statistical model. It is different from probability, as it is not normalized over the parameter space.
Example: For a set of data points $\mathbf{X} = \{x_1, x_2, \ldots, x_n\}$, the likelihood function for a parameter $\theta$ is $L(\theta; \mathbf{X}) = \prod_{i=1}^{n} P(x_i|\theta)$.
PICTURE:
ID: 1718374312130
END

> [!question]- Maximum Likelihood Estimation (MLE)
TARGET DECK: Math::Machine Learning TM
START
Math_ONE_side
TITLE: Maximum Likelihood Estimation (MLE)
DESCRIPTION: 
Maximum Likelihood Estimation (MLE) is a method used to estimate the parameters of a statistical model. It finds the parameter values that maximize the likelihood function given the observed data.
FORMULA: 
$\hat{\theta}_{MLE} = \underset{\theta}{\operatorname{argmax}} \ L(\theta; \mathbf{X})$
ADDITIONAL:
MLE is widely used in various fields, including machine learning, to fit models to data. It provides parameter estimates that are asymptotically unbiased and efficient.
Example: For a normal distribution with unknown mean $\mu$ and variance $\sigma^2$, MLE estimates for $\mu$ and $\sigma^2$ are given by:
$\hat{\mu} = \frac{1}{n} \sum_{i=1}^n x_i$ and $\hat{\sigma}^2 = \frac{1}{n} \sum_{i=1}^n (x_i - \hat{\mu})^2$.
PICTURE:
ID: 1718374312133
END


#### 8. What is cross-validation? How does the number of folds affect the validation?
> [!question]- Cross-Validation Definition
TARGET DECK: Math::Machine Learning TM
START
Math_ONE_side
TITLE: Cross-Validation Definition
DESCRIPTION: 
Cross-validation is a technique for assessing the performance of a machine learning model by partitioning the data into a set of training and validation sets. The model is trained on the training set and validated on the validation set. This process is repeated multiple times to ensure that the model's performance is robust and not dependent on a particular split of the data.
FORMULA: 
N/A
ADDITIONAL:
There are various types of cross-validation, including k-fold, leave-one-out, and stratified cross-validation. K-fold cross-validation is the most common, where the dataset is divided into k subsets (folds). The model is trained on k-1 folds and validated on the remaining fold. This process is repeated k times, with each fold being used as the validation set once.
PICTURE:
ID: 1718374366671
END

> [!question]- Effect of the Number of Folds in Cross-Validation
TARGET DECK: Math::Machine Learning TM
START
Math_ONE_side
TITLE: Effect of the Number of Folds in Cross-Validation
DESCRIPTION: 
The number of folds in cross-validation affects the trade-off between bias and variance in the model's performance estimation. With fewer folds (e.g., 5-fold cross-validation), the training set is larger, which may result in lower variance but higher bias. With more folds (e.g., 10-fold cross-validation), the training set is smaller, which may result in higher variance but lower bias.
FORMULA: 
N/A
ADDITIONAL:
In general, increasing the number of folds provides a more reliable estimate of model performance but at the cost of increased computational expense. Leave-one-out cross-validation (LOOCV) is an extreme case where the number of folds equals the number of data points, offering the lowest bias but highest variance and computational cost.
PICTURE:
ID: 1718374366674
END


#### 9. What is overfitting and underfitting? How to detect them?
> [!question]- Overfitting
TARGET DECK: Math::Machine Learning TM
START
Math_TWO_side
TITLE: Overfitting
DESCRIPTION: 
{TITLE} occurs when a model learns the training data too well, including noise and minor fluctuations, leading to poor generalization to new data.
FORMULA: 
N/A
ADDITIONAL:
Examples of {TITLE}:
- A decision tree with too many branches that captures noise in the data.
- High accuracy on training data but low accuracy on validation or test data.
PICTURE:
ID: 1718374866595
END

> [!question]- Underfitting
TARGET DECK: Math::Machine Learning TM
START
Math_TWO_side
TITLE: Underfitting
DESCRIPTION: 
{TITLE} occurs when a model is too simple to capture the underlying patterns in the data, resulting in high error on both training and validation data.
FORMULA: 
N/A
ADDITIONAL:
Examples of {TITLE}:
- A linear regression model used to fit non-linear data.
- High error on both training and validation data, low accuracy on training data.
PICTURE:
ID: 1718374866598
END

> [!question]- Detecting Overfitting
TARGET DECK: Math::Machine Learning TM
START
Math_ONE_side
TITLE: Detecting Overfitting
DESCRIPTION: 
To detect overfitting, check for high accuracy on training data but low accuracy on validation or test data. Look for a large gap between training and validation error.
FORMULA: 
N/A
ADDITIONAL:
Methods to mitigate {TITLE}:
- Use cross-validation.
- Apply regularization techniques.
- Prune decision trees.
PICTURE:
ID: 1718374866600
END

> [!question]- Detecting Underfitting
TARGET DECK: Math::Machine Learning TM
START
Math_ONE_side
TITLE: Detecting Underfitting
DESCRIPTION: 
To detect underfitting, check for high error on both training and validation data and low accuracy on training data.
FORMULA: 
N/A
ADDITIONAL:
Methods to mitigate {TITLE}:
- Increase model complexity.
- Add more features.
- Reduce regularization.
PICTURE:
ID: 1718374866603
END


#### 10. What is the difference between parameters and hyperparameters? Provide an example for linear models/decision trees.
> [!question]- Parameters
TARGET DECK: Math::Machine Learning TM
START
Math_TWO_side
TITLE: Parameters
DESCRIPTION: 
{TITLE} are internal variables of a model that are learned from the training data. They are adjusted by the learning algorithm to minimize the loss function.
FORMULA: 
None
ADDITIONAL:
For example, in a linear regression model, the coefficients (weights) $\mathbf{w}$ are parameters. In decision trees, the split points for each node are parameters.
PICTURE:
ID: 1718374977195
END

> [!question]- Hyperparameters
TARGET DECK: Math::Machine Learning TM
START
Math_TWO_side
TITLE: Hyperparameters
DESCRIPTION: 
{TITLE} are external variables set before the training process begins. They are not learned from the data but are used to control the learning process.
FORMULA: 
None
ADDITIONAL:
Examples include the learning rate $\alpha$ in gradient descent for linear models, or the maximum depth of a decision tree.
PICTURE:
ID: 1718374977198
END

> [!question]- Difference between Parameters and Hyperparameters
TARGET DECK: Math::Machine Learning TM
START
Math_ONE_side
TITLE: Difference between Parameters and Hyperparameters
DESCRIPTION: 
Parameters are learned from the training data and directly influence the predictions of the model. Hyperparameters are set before training and control the learning process, but they are not directly learned from the data.
FORMULA: 
None
ADDITIONAL:
For linear models, parameters include the weights $\mathbf{w}$, while a hyperparameter example is the learning rate $\alpha$. For decision trees, parameters include the split points at each node, while hyperparameters include the maximum tree depth.
PICTURE:
ID: 1718374977199
END


> [!question]- Parameters
TARGET DECK: Math::Machine Learning TM
START
Math_TWO_side
TITLE: Parameters
DESCRIPTION: 
{TITLE} are internal variables of a model that are learned from the training data. They are adjusted by the learning algorithm to minimize the loss function.
FORMULA: 
None
ADDITIONAL:
For example, in a linear regression model, the coefficients (weights) $\mathbf{w}$ are parameters. In decision trees, the split points for each node are parameters.
PICTURE:
ID: 1733048850829
END

> [!question]- Hyperparameters
TARGET DECK: Math::Machine Learning TM
START
Math_TWO_side
TITLE: Hyperparameters
DESCRIPTION: 
{TITLE} are external variables set before the training process begins. They are not learned from the data but are used to control the learning process.
FORMULA: 
None
ADDITIONAL:
Examples include the learning rate $\alpha$ in gradient descent for linear models, or the maximum depth of a decision tree.
PICTURE:
ID: 1733048850830
END

> [!question]- Difference between Parameters and Hyperparameters
TARGET DECK: Math::Machine Learning TM
START
Math_ONE_side
TITLE: Difference between Parameters and Hyperparameters
DESCRIPTION: 
Parameters are learned from the training data and directly influence the predictions of the model. Hyperparameters are set before training and control the learning process, but they are not directly learned from the data.
FORMULA: 
None
ADDITIONAL:
For linear models, parameters include the weights $\mathbf{w}$, while a hyperparameter example is the learning rate $\alpha$. For decision trees, parameters include the split points at each node, while hyperparameters include the maximum tree depth.
PICTURE:
ID: 1733048850831
END


#### 11. What is a regularization? What is the difference between L1 and L2 regularization in linear models? Is it the only way to constrain the solution?
> [!question]- Regularization
TARGET DECK: Math::Machine Learning TM
START
Math_TWO_side
TITLE: Regularization
DESCRIPTION: 
{TITLE} is a technique used to prevent overfitting by adding a penalty term to the loss function, discouraging the model from becoming too complex.
FORMULA: 
Loss function with regularization: $L(\mathbf{w}) + \lambda R(\mathbf{w})$
ADDITIONAL:
Where $L(\mathbf{w})$ is the original loss function, $\lambda$ is the regularization parameter, and $R(\mathbf{w})$ is the regularization term.
PICTURE:
ID: 1718375422777
END

> [!question]- L1 Regularization
TARGET DECK: Math::Machine Learning TM
START
Math_TWO_side
TITLE: L1 Regularization
DESCRIPTION: 
{TITLE} adds the absolute value of the coefficients as a penalty term to the loss function, encouraging sparse models.
FORMULA: 
$R(\mathbf{w}) = \sum_{i=1}^{n} |\mathbf{w}_i|$
ADDITIONAL:
Example: Lasso Regression can be used for feature selection because it can shrink some coefficients to exactly zero.
PICTURE:
ID: 1718375422780
END

> [!question]- L2 Regularization
TARGET DECK: Math::Machine Learning TM
START
Math_TWO_side
TITLE: L2 Regularization
DESCRIPTION: 
{TITLE} adds the squared value of the coefficients as a penalty term to the loss function, reducing model complexity without necessarily zeroing out coefficients.
FORMULA: 
$R(\mathbf{w}) = \sum_{i=1}^{n} \mathbf{w}_i^2$
ADDITIONAL:
Example: Ridge Regression helps in situations where the number of predictors is large but none is strongly indicative, by shrinking all coefficients.
PICTURE:
ID: 1718375422782
END

> [!question]- Other Methods to Constrain Solutions
TARGET DECK: Math::Machine Learning TM
START
Math_ONE_side
TITLE: Other Methods to Constrain Solutions
DESCRIPTION: 
Other methods to constrain solutions include early stopping, dropout, and data augmentation.
FORMULA: 
None
ADDITIONAL:
- **Early Stopping**: Stops training before overfitting.
- **Dropout**: Randomly drops units during neural network training.
- **Data Augmentation**: Increases training data through transformations.
PICTURE:
ID: 1718375422784
END


#### 12. Does L2 regularization regularize the bias term (w_0 or b)? Why?
> [!question]- Does L2 regularization regularize the bias term (w_0 or b)?
TARGET DECK: Math::Machine Learning TM
START
Math_ONE_side
TITLE: Does L2 regularization regularize the bias term (w_0 or b)?
DESCRIPTION: 
No, {TITLE} typically does not regularize the bias term. The reason is that regularizing the bias term could introduce unnecessary bias into the model, which might affect its ability to fit the data well.
FORMULA: 
$L(\mathbf{w}) = \text{MSE}(\mathbf{w}) + \lambda \sum_{j=1}^{p} w_j^2$
ADDITIONAL:
The regularization term $\lambda \sum_{j=1}^{p} w_j^2$ usually only includes the weights for the features and not the bias term. Regularizing the bias term could shift the predictions uniformly, which is not desirable.
PICTURE:
ID: 1718375533144
END


#### 13. Why is it a good idea to normalize data before applying a linear model?
> [!question]- Normalization
TARGET DECK: Math::Machine Learning TM
START
Math_TWO_side
TITLE: Normalization
DESCRIPTION: 
{TITLE} is a technique used to adjust the values of features in your dataset to a common scale without distorting differences in the ranges of values.
FORMULA: 
$X' = \frac{X - \mu}{\sigma}$
ADDITIONAL:
{TITLE} helps ensure that each feature contributes equally to the model, leading to better performance and faster convergence during training. For example, normalizing features to a range of [0, 1] or to have zero mean and unit variance are common practices.
PICTURE:
ID: 1718375605777
END

> [!question]- Normalization in Linear Models
TARGET DECK: Math::Machine Learning TM
START
Math_TWO_side
TITLE: Normalization in Linear Models
DESCRIPTION: 
{TITLE} is the process of scaling the features of your data so that they have a mean of zero and a standard deviation of one, or so that they fall within a specific range such as 0 to 1.
FORMULA: 
$X' = \frac{X - \mu}{\sigma}$
ADDITIONAL:
{TITLE} helps ensure that each feature contributes equally to the model, speeds up convergence during gradient descent, and prevents numerical instability.
PICTURE:
ID: 1718375605780
END

> [!question]- Benefits of Normalizing Data
TARGET DECK: Math::Machine Learning TM
START
Math_ONE_side
TITLE: Benefits of Normalizing Data
DESCRIPTION: 
Normalizing data ensures that all features contribute equally to the model, speeds up convergence during training, and helps avoid numerical instability.
FORMULA: 
ADDITIONAL:
For example, without normalization, a feature with a larger range can dominate the model coefficients, leading to poor performance. In gradient descent, normalization helps achieve faster and more consistent convergence.
PICTURE:
ID: 1718375605782
END

> [!question]- Formula for Normalization
TARGET DECK: Math::Machine Learning TM
START
Math_ONE_side
TITLE: Formula for Normalization
DESCRIPTION: 
The formula for normalization is given by:
FORMULA: 
$X' = \frac{X - \mu}{\sigma}$
ADDITIONAL:
Where $X$ is the original feature, $\mu$ is the mean of the feature, and $\sigma$ is the standard deviation of the feature.
PICTURE:
ID: 1718375605783
END


#### 14. Provide a linear classification problem statement. What is a margin?
> [!question]- Linear Classification Problem Statement
TARGET DECK: Math::Machine Learning TM
START
Math_ONE_side
TITLE: Linear Classification Problem Statement
DESCRIPTION: 
A linear classification problem involves categorizing data into two or more classes using a linear decision boundary.
FORMULA: 
$\mathbf{w}^\top \mathbf{x} + b = 0$
ADDITIONAL:
Example: Given a dataset of emails, classify each email as either "spam" or "not spam" based on features like word frequency, presence of links, etc.
PICTURE:
ID: 1718375644089
END

> [!question]- Margin in Linear Classification
TARGET DECK: Math::Machine Learning TM
START
Math_TWO_side
TITLE: Margin in Linear Classification
DESCRIPTION: 
{TITLE} refers to the distance between the decision boundary (hyperplane) and the closest data points from any class.
FORMULA: 
Margin = $\frac{2}{\|\mathbf{w}\|}$
ADDITIONAL:
A larger margin indicates better generalization capability. In SVM, the objective is to maximize this margin.
PICTURE:
ID: 1718375644093
END

#### 15. What are precision and recall? How to use them to measure the model quality?
> [!question]- Precision
TARGET DECK: Math::Machine Learning TM
START
Math_TWO_side
TITLE: Precision
DESCRIPTION: 
{TITLE} is a measure of how many of the positive predictions made by the model are actually correct. It is calculated as the ratio of true positives (TP) to the sum of true positives and false positives (FP).
FORMULA: 
$\text{Precision} = \frac{TP}{TP + FP}$
ADDITIONAL:
High precision indicates a low false positive rate. It is particularly important in situations where the cost of false positives is high, such as in spam detection.
PICTURE:
ID: 1718375687316
END

> [!question]- Recall
TARGET DECK: Math::Machine Learning TM
START
Math_TWO_side
TITLE: Recall
DESCRIPTION: 
{TITLE} is a measure of how many of the actual positive cases the model correctly identified. It is calculated as the ratio of true positives (TP) to the sum of true positives and false negatives (FN).
FORMULA: 
$\text{Recall} = \frac{TP}{TP + FN}$
ADDITIONAL:
High recall indicates a low false negative rate. It is crucial in scenarios where missing a positive case is costly, such as in medical diagnoses.
PICTURE:
ID: 1718375687320
END

> [!question]- Using Precision and Recall to Measure Model Quality
TARGET DECK: Math::Machine Learning TM
START
Math_ONE_side
TITLE: Using Precision and Recall to Measure Model Quality
DESCRIPTION: 
Precision and recall are often used together to measure the quality of a model. The balance between precision and recall can be adjusted based on the specific needs of the application. One common way to combine them is through the F1 score, which is the harmonic mean of precision and recall.
FORMULA: 
$F1 = 2 \cdot \frac{\text{Precision} \cdot \text{Recall}}{\text{Precision} + \text{Recall}}$
ADDITIONAL:
High F1 score indicates that the model has both high precision and high recall. This is particularly useful when you need a balance between precision and recall.
PICTURE:
ID: 1718375687321
END


#### 16. Assume the dataset for binary classification is imbalanced, so 95% of data belong to the first class. How to adjust the classification quality measures, to work with such data? Why?
> [!question]- Imbalanced Dataset Problem in Binary Classification
TARGET DECK: Math::Machine Learning TM
START
Math_TWO_side
TITLE: Imbalanced Dataset Problem in Binary Classification
DESCRIPTION: 
{TITLE} occurs when one class significantly outnumbers the other, leading to misleading performance metrics and potentially poor model performance on the minority class.
FORMULA: 
ADDITIONAL:
Problem:
In a dataset where 95% of the data belong to one class, a classifier that always predicts the majority class would achieve 95% accuracy but fail to identify any instances of the minority class.
Solutions:
1. **Precision-Recall Curve:**
   - More informative than the ROC curve for imbalanced datasets because it focuses on the performance of the positive class.
   - Precision = $\frac{TP}{TP + FP}$, Recall = $\frac{TP}{TP + FN}$
2. **Use Metrics like F1 Score:**
   - Harmonic mean of precision and recall, balancing both concerns.
   - $F1 = 2 \cdot \frac{Precision \cdot Recall}{Precision + Recall}$
3. **Class Weights:**
   - Adjust class weights in the classifier to assign a higher penalty to misclassifying the minority class.
   - In many machine learning libraries, setting `class_weight` to 'balanced' can automatically adjust the weights inversely proportional to class frequencies.
4. **Resampling Techniques:**
   - Oversampling the minority class or undersampling the majority class can help balance the dataset.
   - Techniques such as SMOTE (Synthetic Minority Over-sampling Technique) can generate synthetic samples for the minority class.
PICTURE:
ID: 1718375812592
END

> [!question]- Precision-Recall Curve
TARGET DECK: Math::Machine Learning TM
START
Math_TWO_side
TITLE: Precision-Recall Curve
DESCRIPTION: 
{TITLE} is more informative than the ROC curve for imbalanced datasets because it focuses on the performance of the positive class.
FORMULA: 
Precision = $\frac{TP}{TP + FP}$, Recall = $\frac{TP}{TP + FN}$
ADDITIONAL:
TP: True Positives, FP: False Positives, FN: False Negatives. {TITLE} helps in understanding the trade-off between precision and recall.
PICTURE:
ID: 1718375824521
END

> [!question]- F1 Score
TARGET DECK: Math::Machine Learning TM
START
Math_TWO_side
TITLE: F1 Score
DESCRIPTION: 
{TITLE} is the harmonic mean of precision and recall, providing a single measure that balances both concerns.
FORMULA: 
$F1 = 2 \cdot \frac{Precision \cdot Recall}{Precision + Recall}$
ADDITIONAL:
{TITLE} is particularly useful when the class distribution is imbalanced.
PICTURE:
ID: 1718375824524
END

> [!question]- Class Weights
TARGET DECK: Math::Machine Learning TM
START
Math_ONE_side
TITLE: Class Weights
DESCRIPTION: 
Adjusting class weights in the classifier helps to handle class imbalance by assigning a higher penalty to misclassifying the minority class.
FORMULA: 
ADDITIONAL:
In many machine learning libraries, setting `class_weight` to 'balanced' can automatically adjust the weights inversely proportional to class frequencies.
PICTURE:
ID: 1718375824526
END

> [!question]- Resampling Techniques
TARGET DECK: Math::Machine Learning TM
START
Math_ONE_side
TITLE: Resampling Techniques
DESCRIPTION: 
Resampling techniques like oversampling the minority class or undersampling the majority class can help balance the dataset.
FORMULA: 
ADDITIONAL:
Techniques such as SMOTE (Synthetic Minority Over-sampling Technique) can generate synthetic samples for the minority class.
PICTURE:
ID: 1718375824528
END


#### 17. What is ROC AUC? How to build the ROC curve?
> [!question]- ROC Curve
TARGET DECK: Math::Machine Learning TM
START
Math_TWO_side
TITLE: ROC Curve
DESCRIPTION: 
{TITLE} is a graphical plot used to illustrate the diagnostic ability of a binary classifier system as its discrimination threshold is varied. It plots the True Positive Rate (TPR) against the False Positive Rate (FPR).
FORMULA: 
TPR = $\frac{TP}{TP + FN}$, FPR = $\frac{FP}{FP + TN}$
ADDITIONAL:
The ROC curve helps visualize the trade-off between sensitivity (TPR) and specificity (1 - FPR). An ideal classifier has a point at (0,1). The closer the ROC curve is to the top-left corner, the better the classifier's performance.
PICTURE:
ID: 1718375938546
END

> [!question]- ROC AUC
TARGET DECK: Math::Machine Learning TM
START
Math_TWO_side
TITLE: ROC AUC
DESCRIPTION: 
{TITLE} is a performance metric for binary classifiers represented as the area under the ROC curve. It reflects the classifier's ability to distinguish between classes.
FORMULA: 
AUC (Area Under the Curve) is calculated based on the ROC curve which plots TPR against FPR.
ADDITIONAL:
An AUC of 0.5 indicates random performance, while an AUC of 1.0 indicates perfect classification. The ROC curve is constructed by plotting the True Positive Rate (TPR) against the False Positive Rate (FPR) at various threshold settings.
PICTURE:
ID: 1718375938550
END

> [!question]- Building the ROC Curve
TARGET DECK: Math::Machine Learning TM
START
Math_ONE_side
TITLE: Building the ROC Curve
DESCRIPTION: 
To build the ROC curve, various threshold values are used to compute the True Positive Rate (TPR) and False Positive Rate (FPR) and plot TPR against FPR.
FORMULA: 
TPR = $\frac{TP}{TP + FN}$, FPR = $\frac{FP}{FP + TN}$
ADDITIONAL:
The ROC curve helps visualize the trade-off between sensitivity (TPR) and specificity (1 - FPR). It is particularly useful for comparing different classifiers.
PICTURE:
ID: 1718375938553
END


#### 18. Logistic loss function. How is it related to Maximum likelihood estimation?
> [!question]- Logistic Loss Function
TARGET DECK: Math::Machine Learning TM
START
Math_TWO_side
TITLE: Logistic Loss Function
DESCRIPTION: 
{TITLE} is used in logistic regression to measure the performance of a classification model. It quantifies the difference between the predicted probabilities and the actual labels.
FORMULA: 
$L(\mathbf{w}) = -\frac{1}{n} \sum_{i=1}^{n} \left[y_i \log(p_i) + (1 - y_i) \log(1 - p_i)\right]$
ADDITIONAL:
Here, $y_i$ is the actual label, $p_i = \sigma(\mathbf{x}_i^\top \mathbf{w})$ is the predicted probability, and $\sigma(z) = \frac{1}{1 + e^{-z}}$ is the sigmoid function.
PICTURE:
ID: 1718375991894
END

> [!question]- Relationship between Logistic Loss Function and MLE
TARGET DECK: Math::Machine Learning TM
START
Math_TWO_side
TITLE: Relationship between Logistic Loss Function and MLE
DESCRIPTION: 
The {TITLE} is that minimizing the logistic loss function is equivalent to maximizing the likelihood of the observed data under the logistic model. Thus, logistic regression can be seen as an application of MLE.
FORMULA: 
$L(\mathbf{w}) = -\log \left[\prod_{i=1}^{n} P(y_i | \mathbf{x}_i; \mathbf{w}) \right]$
ADDITIONAL:
Minimizing the logistic loss function is the same as minimizing the negative log-likelihood of the data, which is a common approach in MLE.
PICTURE:
ID: 1718375991896
END

> [!question]- Maximum Likelihood Estimation (MLE)
TARGET DECK: Math::Machine Learning TM
START
Math_TWO_side
TITLE: Maximum Likelihood Estimation (MLE)
DESCRIPTION: 
{TITLE} is a method used to estimate the parameters of a statistical model by maximizing the likelihood function, which measures how well the model explains the observed data.
FORMULA: 
$\hat{\mathbf{w}}_{MLE} = \arg \max_{\mathbf{w}} \prod_{i=1}^{n} P(y_i | \mathbf{x}_i; \mathbf{w})$
ADDITIONAL:
For logistic regression, the likelihood function is $P(y_i | \mathbf{x}_i; \mathbf{w}) = p_i^{y_i} (1 - p_i)^{1 - y_i}$, where $p_i = \sigma(\mathbf{x}_i^\top \mathbf{w})$.
PICTURE:
ID: 1718376031791
END


#### 19. Support Vector Machine main idea. The optimization functional for linearly separable case.
> [!question]- Support Vector Machine Main Idea
TARGET DECK: Math::Machine Learning TM
START
Math_TWO_side
TITLE: Support Vector Machine Main Idea
DESCRIPTION: 
{TITLE} is a supervised learning model used for classification and regression. Its main idea is to find the optimal hyperplane that best separates the classes in a dataset.
FORMULA: 
None
ADDITIONAL:
The optimal hyperplane is the one that maximizes the margin between the classes, which is the distance between the closest points (support vectors) of the classes to the hyperplane.
PICTURE:
ID: 1718376095793
END

> [!question]- Optimization Functional for Linearly Separable Case
TARGET DECK: Math::Machine Learning TM
START
Math_TWO_side
TITLE: Optimization Functional for Linearly Separable Case
DESCRIPTION: 
{TITLE} aims to find a hyperplane that separates the data with the maximum margin while minimizing classification errors.
FORMULA: 
$\min_{\mathbf{w}, b} \frac{1}{2} \|\mathbf{w}\|^2 \quad \text{subject to} \quad y_i (\mathbf{w}^\top \mathbf{x}_i + b) \geq 1, \forall i$
ADDITIONAL:
Where $\mathbf{w}$ is the weight vector, $b$ is the bias term, $\mathbf{x}_i$ are the input vectors, and $y_i$ are the corresponding class labels. The constraints ensure that each data point is correctly classified with a margin of at least 1.
PICTURE:
ID: 1718376095795
END


#### 20. Describe the greedy optimization algorithm for the decision tree.

> [!question]- Greedy Optimization Algorithm for Decision Tree
TARGET DECK: Math::Machine Learning TM
START
Math_TWO_side
TITLE: Greedy Optimization Algorithm for Decision Tree
DESCRIPTION: 
{TITLE} is an approach where the algorithm makes the optimal choice at each node with the hope of finding the global optimum. 
FORMULA: 
None
ADDITIONAL:
{TITLE} selects the split at each node that maximizes information gain or minimizes impurity (e.g., Gini index, entropy) based on the available features.
PICTURE:
ID: 1718376149548
END

> [!question]- Information Gain in Decision Trees
TARGET DECK: Math::Machine Learning TM
START
Math_ONE_side
TITLE: Information Gain in Decision Trees
DESCRIPTION: 
Information gain measures the reduction in entropy or impurity from a split.
FORMULA: 
$IG(T, a) = H(T) - \sum_{v \in Values(a)} \frac{|T_v|}{|T|} H(T_v)$
ADDITIONAL:
Where $H(T)$ is the entropy of the set $T$, $a$ is the attribute, $T_v$ is the subset of examples for which attribute $a$ has value $v$, and $|T|$ is the number of elements in set $T$. 
PICTURE:
ID: 1718376149553
END

> [!question]- Gini Index in Decision Trees
TARGET DECK: Math::Machine Learning TM
START
Math_ONE_side
TITLE: Gini Index in Decision Trees
DESCRIPTION: 
The Gini Index is a measure of impurity or impurity for a set of examples.
FORMULA: 
$Gini(T) = 1 - \sum_{i=1}^{n} p_i^2$
ADDITIONAL:
Where $p_i$ is the proportion of examples belonging to class $i$ in set $T$.
PICTURE:
ID: 1718376149555
END

#### 21. Why can an unconstrained decision tree achieve zero error on the training set with unique objects?
> [!question]- Overfitting in Decision Trees
TARGET DECK: Math::Machine Learning TM
START
Math_TWO_side
TITLE: Overfitting in Decision Trees
DESCRIPTION: 
{TITLE} occurs when a decision tree model is too complex and captures the noise in the training data, leading to poor generalization to new data.
FORMULA: 
ADDITIONAL:
An unconstrained decision tree can achieve zero error on the training set with unique objects by creating a separate leaf for each object.
PICTURE:
ID: 1718376194891
END

> [!question]- Unconstrained Decision Tree
TARGET DECK: Math::Machine Learning TM
START
Math_ONE_side
TITLE: Unconstrained Decision Tree
DESCRIPTION: 
An {TITLE} is a decision tree that is allowed to grow without any limitations, such as maximum depth or minimum samples per leaf.
FORMULA: 
ADDITIONAL:
An unconstrained decision tree can achieve zero error on the training set with unique objects by creating a separate leaf for each object. This leads to overfitting.
PICTURE:
ID: 1718376194895
END


#### 22. How to assign a class label for the object in the tree leaf in classification?
> [!question]- Assigning Class Label in Classification
TARGET DECK: Math::Machine Learning TM
START
Math_ONE_side
TITLE: Assigning Class Label in Classification
DESCRIPTION: 
In classification, the class label for an object is assigned based on the majority class of the objects in the tree leaf where the object falls.
FORMULA: 
N/A
ADDITIONAL:
For example, if a leaf contains 10 samples where 7 belong to class A and 3 belong to class B, the object will be assigned class A.
PICTURE:
ID: 1718376243388
END

> [!question]- Assigning Class Label in Decision Trees
TARGET DECK: Math::Machine Learning TM
START
Math_TWO_side
TITLE: Assigning Class Label in Decision Trees
DESCRIPTION: 
{TITLE} involves determining the class label of an object based on the majority class of the samples that reach the same leaf node.
FORMULA: 
N/A
ADDITIONAL:
For instance, if a leaf node contains samples with the following distribution:
- Class 0: 4 samples
- Class 1: 6 samples
The object will be assigned class 1 because it is the majority class.
PICTURE:
ID: 1718376243389
END


#### 23. How to assign a class label for the object in the tree leaf in regression? Does it depend on the information criterion?
> [!question]- Decision Tree Regression
TARGET DECK: Math::Machine Learning TM
START
Math_TWO_side
TITLE: Decision Tree Regression
DESCRIPTION: 
{TITLE} is a decision analysis technique used for predictive modeling that maps observations about an item to conclusions about its target value.
FORMULA: 
N/A
ADDITIONAL:
In {TITLE}, the data is continuously split according to a certain parameter. The end result is a tree with decision nodes and leaf nodes. The leaf nodes contain the predicted value.
PICTURE:
ID: 1718378243307
END

> [!question]- Assigning Class Labels in Regression Trees
TARGET DECK: Math::Machine Learning TM
START
Math_TWO_side
TITLE: Assigning Class Labels in Regression Trees
DESCRIPTION: 
{TITLE} involves determining the output value for a leaf node based on the average or majority value of the training samples that reach that leaf.
FORMULA: 
N/A
ADDITIONAL:
For regression, the prediction for a given leaf is typically the mean of the target values in that leaf. This method helps to minimize the mean squared error (MSE).
PICTURE:
ID: 1718378243310
END

> [!question]- Information Criteria in Decision Trees
TARGET DECK: Math::Machine Learning TM
START
Math_TWO_side
TITLE: Information Criteria in Decision Trees
DESCRIPTION: 
{TITLE} are used to evaluate the quality of splits in the tree. Common criteria include Gini impurity, entropy, and mean squared error (MSE).
FORMULA: 
N/A
ADDITIONAL:
For regression trees, the MSE is often used as the information criterion to measure the quality of the split. Lower MSE indicates a better split.
PICTURE:
ID: 1718378243312
END



#### 24. What is bagging?
> [!question]- Bagging
TARGET DECK: Math::Machine Learning TM
START
Math_TWO_side
TITLE: Bagging
DESCRIPTION: 
{TITLE} is an ensemble learning technique that uses multiple versions of a training dataset created through bootstrapping (random sampling with replacement). Each model is trained on a different subset, and their predictions are aggregated (usually by averaging or voting) to form the final prediction.
FORMULA: 
ADDITIONAL:
- {TITLE} helps reduce variance and prevent overfitting.
- Used in algorithms like Random Forest.
- Aggregation can be done through methods like averaging (for regression) or majority voting (for classification).
- Example: In a Random Forest, multiple decision trees are trained on bootstrapped datasets, and their predictions are aggregated to improve accuracy.
PICTURE:
ID: 1718378286276
END

> [!question]- Bagging in Practice
TARGET DECK: Math::Machine Learning TM
START
Math_ONE_side
TITLE: Bagging in Practice
DESCRIPTION: 
To implement {TITLE}, follow these steps:
1. Create multiple bootstrap samples from the original dataset.
2. Train a separate model on each bootstrap sample.
3. Aggregate the predictions from all models.
FORMULA: 
ADDITIONAL:
- Example: For a dataset with 100 observations, create 10 bootstrap samples with replacement, train 10 separate models, and then average their predictions.
PICTURE:
ID: 1718378286277
END


#### 25. What is Random Forest? How does it differ from Bagging over decision trees?
> [!question]- Random Forest
TARGET DECK: Math::Machine Learning TM
START
Math_TWO_side
TITLE: Random Forest
DESCRIPTION: 
{TITLE} is an ensemble learning method that constructs multiple decision trees during training and outputs the mode of the classes (classification) or mean prediction (regression) of the individual trees.
FORMULA: 
None
ADDITIONAL:
{TITLE} uses bootstrapping (sampling with replacement) to create different datasets for each tree and introduces randomness in the selection of features at each split to ensure that the trees are not correlated.
PICTURE:
ID: 1718378357649
END

> [!question]- Difference between Random Forest and Bagging over Decision Trees
TARGET DECK: Math::Machine Learning TM
START
Math_ONE_side
TITLE: Difference between Random Forest and Bagging over Decision Trees
DESCRIPTION: 
While both Random Forest and Bagging involve creating multiple decision trees using bootstrapped datasets, {TITLE} introduces an additional layer of randomness by selecting a random subset of features for each split in the decision trees.
FORMULA: 
None
ADDITIONAL:
Random Forest aims to reduce the correlation between individual trees by selecting random subsets of features, whereas Bagging uses all features for each split, which can lead to similar trees and less diversity in the ensemble.
PICTURE:
ID: 1718378357653
END


#### 26. How are base algorithms being trained in gradient boosting?
> [!question]- Base Algorithm Training in Gradient Boosting
TARGET DECK: Math::Machine Learning TM
START
Math_TWO_side
TITLE: Base Algorithm Training in Gradient Boosting
DESCRIPTION: 
{TITLE} is a sequential process where each base algorithm is trained to correct the errors of the previous ones. It involves fitting the base learners to the negative gradient of the loss function with respect to the predictions of the ensemble.
FORMULA: 
$\mathbf{F}_m(\mathbf{x}) = \mathbf{F}_{m-1}(\mathbf{x}) + \alpha_m h_m(\mathbf{x})$
ADDITIONAL:
Here, $\mathbf{F}_m(\mathbf{x})$ is the updated prediction, $\mathbf{F}_{m-1}(\mathbf{x})$ is the prediction from the previous model, $\alpha_m$ is the learning rate, and $h_m(\mathbf{x})$ is the m-th base learner fitted to the pseudo-residuals. The pseudo-residuals are the negative gradients of the loss function with respect to the current predictions.
PICTURE:
ID: 1718378437448
END

> [!question]- Example of Gradient Boosting Training Process
TARGET DECK: Math::Machine Learning TM
START
Math_ONE_side
TITLE: Example of Gradient Boosting Training Process
DESCRIPTION: 
In gradient boosting, each subsequent model is trained to predict the residuals of the previous model to improve accuracy. For instance, if we start with an initial prediction $\mathbf{F}_0(\mathbf{x})$, the first base learner $h_1(\mathbf{x})$ is trained on the residuals of $\mathbf{F}_0(\mathbf{x})$.
FORMULA: 
$\mathbf{r}_i^{(0)} = y_i - \mathbf{F}_0(\mathbf{x}_i)$
ADDITIONAL:
The process continues iteratively, where $\mathbf{F}_m(\mathbf{x}) = \mathbf{F}_{m-1}(\mathbf{x}) + \alpha h_m(\mathbf{x})$ and $\mathbf{r}_i^{(m)} = y_i - \mathbf{F}_m(\mathbf{x}_i)$. Each base learner $h_m(\mathbf{x})$ is fitted to these residuals $\mathbf{r}_i^{(m-1)}$.
PICTURE:
ID: 1718378437451
END


#### 27. How does backpropagation work in neural networks? What will be vector by vector derivative?
> [!question]- Backpropagation in Neural Networks
TARGET DECK: Math::Machine Learning TM
START
Math_TWO_side
TITLE: Backpropagation
DESCRIPTION: 
{TITLE} is an algorithm for training feedforward neural networks. It involves a forward pass to calculate the output and a backward pass to compute the gradient of the loss with respect to each weight using the chain rule. This gradient is then used to update the weights to minimize the error.
FORMULA: 
The weight update rule: $\mathbf{W} := \mathbf{W} - \alpha \nabla L(\mathbf{W})$
ADDITIONAL:
The process involves calculating the derivative of the loss function with respect to each weight, $\frac{\partial L}{\partial \mathbf{W}}$, which is done using the chain rule.
PICTURE:
ID: 1718378449201
END

> [!question]- Vector by Vector Derivative in Backpropagation
TARGET DECK: Math::Machine Learning TM
START
Math_ONE_side
TITLE: Vector by Vector Derivative in Backpropagation
DESCRIPTION: 
In backpropagation, the vector by vector derivative refers to the calculation of the gradient of the loss function with respect to the weights for each layer in a neural network.
FORMULA: 
$\frac{\partial L}{\partial \mathbf{W}} = \frac{\partial L}{\partial \mathbf{z}} \frac{\partial \mathbf{z}}{\partial \mathbf{W}}$
ADDITIONAL:
Where $\mathbf{z}$ is the pre-activation of the neurons. For a layer with activation function $f$ and weights $\mathbf{W}$, the gradient for the weights is computed as:
$$\frac{\partial L}{\partial \mathbf{W}} = \delta \mathbf{a}^\top $$
where $\delta = \frac{\partial L}{\partial \mathbf{a}} \cdot f'(\mathbf{z})$ and $\mathbf{a}$ is the activation from the previous layer.
PICTURE:
ID: 1718378449202
END


#### 28. How does the Convolutional layer work? What is the convolution operation?
> [!question]- Convolutional Layer in CNN
TARGET DECK: Math::Machine Learning TM
START
Math_TWO_side
TITLE: Convolutional Layer in CNN
DESCRIPTION: 
{TITLE} is a type of layer in a convolutional neural network that applies a convolution operation to the input, passing the result to the next layer. It is designed to automatically and adaptively learn spatial hierarchies of features from input images.
FORMULA: 
$y_{i,j}^{k} = \sum_{m,n} x_{i+m,j+n} \cdot w_{m,n}^{k} + b^{k}$
ADDITIONAL:
In the formula, $y_{i,j}^{k}$ is the output feature map, $x_{i+m,j+n}$ is the input image, $w_{m,n}^{k}$ is the filter (or kernel), and $b^{k}$ is the bias term. The convolutional layer helps in reducing the number of parameters and avoids overfitting.
PICTURE:
ID: 1718378514402
END

> [!question]- Convolution Operation
TARGET DECK: Math::Machine Learning TM
START
Math_TWO_side
TITLE: Convolution Operation
DESCRIPTION: 
{TITLE} is a mathematical operation used in the convolutional layer of a CNN. It involves sliding a filter over the input data to produce a feature map.
FORMULA: 
$y(i,j) = \sum_{m,n} x(i+m,j+n) \cdot w(m,n)$
ADDITIONAL:
The convolution operation detects features such as edges, textures, and patterns in the input image. The filter is also known as the kernel, and it learns to identify specific features through training.
PICTURE:
ID: 1718378514405
END


#### 29. Why fully connected (dense) networks are not the best choice to work with image data? Why do CNNs perform better?
> [!question]- Fully Connected Networks and Image Data
TARGET DECK: Math::Machine Learning TM
START
Math_ONE_side
TITLE: Fully Connected Networks and Image Data
DESCRIPTION: 
Fully connected networks (dense networks) are not ideal for image data because they do not account for the spatial structure of images. Each neuron in a dense layer is connected to every neuron in the previous layer, which leads to a large number of parameters and makes the network prone to overfitting.
FORMULA: 
None
ADDITIONAL:
- Dense networks treat each pixel independently, ignoring the spatial relationships between pixels.
- This leads to a high computational cost and memory usage.
- They are less efficient in capturing local patterns in images.
PICTURE:
ID: 1718378663797
END

> [!question]- Convolutional Neural Networks (CNNs) for Image Data
TARGET DECK: Math::Machine Learning TM
START
Math_TWO_side
TITLE: Convolutional Neural Networks (CNNs) for Image Data
DESCRIPTION: 
{TITLE} are specifically designed to process and analyze visual data by taking advantage of the spatial structure of images. They use convolutional layers to automatically and adaptively learn spatial hierarchies of features.
FORMULA: 
$\text{Feature Map} = \sigma(\mathbf{W} * \mathbf{X} + \mathbf{b})$
ADDITIONAL:
- The convolution operation preserves the spatial relationship between pixels.
- CNNs use pooling layers to reduce the dimensionality and computational complexity.
- They are less prone to overfitting due to fewer parameters compared to fully connected networks.
- Example: In image classification, CNNs can detect edges, textures, and shapes in the initial layers, and more complex patterns in deeper layers.
PICTURE:
ID: 1718378663799
END

#### 30. How does basic RNN (Vanilla RNN) work?
> [!question]- Basic RNN (Vanilla RNN): Introduction
TARGET DECK: Math::Machine Learning TM
START
Math_TWO_side
TITLE: Basic RNN (Vanilla RNN)
DESCRIPTION: 
{TITLE} is a type of neural network designed for sequence data, where each neuron maintains an internal state that can capture information from previous time steps.
FORMULA: 
$h_t = \sigma(W_{hh} h_{t-1} + W_{xh} x_t + b_h)$
ADDITIONAL:
- $h_t$: hidden state at time step $t$
- $x_t$: input at time step $t$
- $W_{hh}$: weight matrix for hidden state
- $W_{xh}$: weight matrix for input
- $b_h$: bias term
- $\sigma$: activation function (commonly tanh or ReLU)
PICTURE:
ID: 1718378684798
END

> [!question]- Basic RNN (Vanilla RNN): Forward Propagation
TARGET DECK: Math::Machine Learning TM
START
Math_ONE_side
TITLE: Forward Propagation in RNN
DESCRIPTION: 
In RNN, forward propagation involves calculating the hidden state for each time step based on the current input and the previous hidden state.
FORMULA: 
$h_t = \sigma(W_{hh} h_{t-1} + W_{xh} x_t + b_h)$
ADDITIONAL:
- The output at each time step can be computed as $y_t = W_{hy} h_t + b_y$, where $W_{hy}$ is the weight matrix for the output and $b_y$ is the bias term.
PICTURE:
ID: 1718378684801
END

> [!question]- Basic RNN (Vanilla RNN): Training with Backpropagation Through Time (BPTT)
TARGET DECK: Math::Machine Learning TM
START
Math_TWO_side
TITLE: Training with Backpropagation Through Time (BPTT)
DESCRIPTION: 
{TITLE} is a technique used to train RNNs by unrolling the network through time and applying backpropagation to compute gradients.
FORMULA: 
$\frac{\partial L}{\partial \theta} = \sum_{t=1}^{T} \frac{\partial L_t}{\partial \theta}$
ADDITIONAL:
- $\theta$ represents the parameters of the RNN.
- The loss $L$ is computed over all time steps.
- Gradients are calculated for each time step and summed to update the weights.
- This process can be computationally expensive and suffers from vanishing/exploding gradient problems.
PICTURE:
ID: 1718378684802
END

> [!question]- Basic RNN (Vanilla RNN): Vanishing and Exploding Gradients
TARGET DECK: Math::Machine Learning TM
START
Math_TWO_side
TITLE: Vanishing and Exploding Gradients in RNNs
DESCRIPTION: 
{TITLE} are common issues in training RNNs where gradients either diminish or grow exponentially, making training difficult.
FORMULA: 
N/A
ADDITIONAL:
- Vanishing gradients: The gradients become very small, causing the network to learn very slowly.
- Exploding gradients: The gradients become very large, causing the network to become unstable.
- Solutions include gradient clipping, using different architectures like LSTM or GRU.
PICTURE:
ID: 1718378684804
END


#### 31. How does dropout work?
#### 32. How do dropout and batch normalization change their behaviour on the inference stage?
> [!question]- Dropout in Inference Stage
TARGET DECK: Math::Machine Learning TM
START
Math_ONE_side
TITLE: Dropout in Inference Stage
DESCRIPTION: 
During the inference stage, dropout is turned off, and the full network is used for making predictions. The weights are scaled appropriately to account for the training phase dropout.
FORMULA: 
None
ADDITIONAL:
In the training phase, some neurons are randomly deactivated to prevent overfitting. However, in the inference phase, all neurons are active, and the weights are scaled by the dropout probability to maintain the expected output.
PICTURE:
ID: 1718378766140
END

> [!question]- Batch Normalization in Inference Stage
TARGET DECK: Math::Machine Learning TM
START
Math_ONE_side
TITLE: Batch Normalization in Inference Stage
DESCRIPTION: 
During the inference stage, batch normalization uses the running mean and variance computed during training instead of the current batch statistics to normalize the input of each layer.
FORMULA: 
None
ADDITIONAL:
In the training phase, batch normalization normalizes the input using the mean and variance of the current batch to stabilize and accelerate training. However, in the inference phase, the running mean and variance calculated during training are used to ensure consistent and accurate predictions.
PICTURE:
ID: 1718378766142
END


#### 33. What is the problem statement for the Principal Component Analysis?

> [!question]- Principal Component Analysis
TARGET DECK: Math::Machine Learning TM
START
Math_TWO_side
TITLE: Principal Component Analysis
DESCRIPTION: 
{TITLE} is a statistical procedure that uses orthogonal transformation to convert a set of possibly correlated variables into a set of linearly uncorrelated variables called principal components.
FORMULA: 
$\mathbf{Z} = \mathbf{X} \mathbf{W}$
ADDITIONAL:
The principal components are ordered by the amount of variance they capture from the data. The first principal component captures the most variance, followed by the second, and so on.
PICTURE:
ID: 1718378800167
END

> [!question]- Problem Statement for Principal Component Analysis
TARGET DECK: Math::Machine Learning TM
START
Math_ONE_side
TITLE: Problem Statement for Principal Component Analysis
DESCRIPTION: 
The problem statement for {TITLE} involves finding a new set of orthogonal axes such that the projection of the data onto these axes maximizes the variance, thereby reducing the dimensionality of the data while retaining as much variability as possible.
FORMULA: 
$\mathbf{W} = \arg \max_{\mathbf{W}} \text{Var}(\mathbf{XW})$
ADDITIONAL:
This is achieved by calculating the eigenvectors and eigenvalues of the covariance matrix of the data, where the eigenvectors form the new axes and the eigenvalues indicate the amount of variance captured by each axis.
PICTURE:
ID: 1718378800170
END


