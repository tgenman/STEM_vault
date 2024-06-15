---
aliases: 
publish: true
created: 2024-06-08 10:43
connected:
  - "[[Machine Learning MOC]]"
  - "[[Вастрик - Машинное обучение]]"
---

[[Machine Learning exam Theoretical minimum]]


#### 0. Machine Learning problem statement. Regression, Classification, examples.

> [!question]- Machine Learning Problem Statement
TARGET DECK: Math::Machine Learning 0
START
Math_ONE_side
TITLE: Machine Learning Problem Statement
DESCRIPTION: A machine learning problem statement defines the task to be solved using algorithms that learn from data. It typically includes the type of problem (e.g., regression, classification), the desired output, and the evaluation criteria.
FORMULA: 
ADDITIONAL: 
> Examples of problem statements:
> - Predicting house prices (regression)
> - Classifying emails as spam or not spam (classification)
PICTURE:
ID: 1717827029210
END

> [!question]- Regression
TARGET DECK: Math::Machine Learning 0
START
Math_TWO_side
TITLE: Regression
DESCRIPTION: Regression is a type of machine learning task where the goal is to predict a continuous-valued output based on input features.
FORMULA: \$y = f(X) + \epsilon$
ADDITIONAL: 
Common examples:
- Predicting the price of a house based on its features (size, location, etc.)
- Predicting the temperature for the next day based on historical data
PICTURE: ![[Pasted image 20230503121619.png|300]]
ID: 1717827133046
END

> [!question]- Classification
TARGET DECK: Math::Machine Learning 0
START
Math_TWO_side
TITLE: Classification
DESCRIPTION: Classification is a type of machine learning task where the goal is to predict a discrete label or category for a given input based on its features.
FORMULA: $\hat{y} = \arg \max_{c \in C} P(c|X)$
ADDITIONAL: 
Common examples:
- Classifying emails as spam or not spam
- Diagnosing medical conditions based on patient data
PICTURE: ![[Pasted image 20230503110504.png|300]]
ID: 1717827133049
END


#### 3. Maximum likelihood estimation, how is it related to regression and classification

> [!question]-
TARGET DECK: Math::Machine Learning 0
START
Math_TWO_side
TITLE: Maximum Likelihood Estimation (MLE)
DESCRIPTION: 
Maximum likelihood estimation (MLE) is a method of estimating the parameters of a statistical model. It is based on maximizing the likelihood function, which measures how well the model explains the observed data.
FORMULA: 
The likelihood function $L(\theta)$ for a given dataset $X$ and parameter $\theta$ is:
$L(\theta) = P(X | \theta)$
The MLE is the value of $\theta$ that maximizes $L(\theta)$:
$\hat{\theta} = \arg \max_{\theta} L(\theta)$
ADDITIONAL:
Example: 
- In regression, MLE can be used to estimate the coefficients of the model by maximizing the likelihood of the observed data given the model.
- In classification, MLE can be used to estimate the parameters of the probability distribution for each class.
PICTURE:
ID: 1717827476515
END

> [!question]-
TARGET DECK: Math::Machine Learning 0
START
Math_ONE_side
TITLE: MLE in Regression
DESCRIPTION: 
In regression, MLE is used to find the parameter values that make the observed data most probable under the assumed model. For example, in linear regression, MLE can estimate the coefficients by maximizing the likelihood of the observed data given the model.
FORMULA: 
The likelihood function for linear regression:
$L(\beta) = \prod_{i=1}^{n} P(y_i | x_i, \beta)$
The MLE is:
$\hat{\beta} = \arg \max_{\beta} L(\beta)$
ADDITIONAL:
Example: 
- For a linear regression model $y = \beta_0 + \beta_1 x$, the MLE estimates $\beta_0$ and $\beta_1$ by maximizing the likelihood function.
PICTURE:
ID: 1717827476520
END


> [!question]-
TARGET DECK: Math::Machine Learning 0
START
Math_ONE_side
TITLE: MLE in Classification
DESCRIPTION: 
In classification, MLE is used to estimate the parameters of the probability distribution for each class. This involves maximizing the likelihood function for the observed data given the class labels.
FORMULA: 
The likelihood function for classification:
$L(\theta) = \prod_{i=1}^{n} P(y_i | x_i, \theta)$
The MLE is:
$\hat{\theta} = \arg \max_{\theta} L(\theta)$
ADDITIONAL:
Example: 
- In logistic regression, MLE estimates the coefficients of the logistic function by maximizing the likelihood of the observed class labels given the input data.
PICTURE:
ID: 1717827476524
END


#### 6. Linear regression. Problem statement for the MSE loss function case. Analytical solution. Gauss-Markov theorem. Gradient approach in linear regression.

> [!question]- Problem Statement for the MSE Loss Function Case
TARGET DECK: Math::Machine Learning 0
START
Math_ONE_side
TITLE: Problem Statement for the MSE Loss Function Case
DESCRIPTION: 
The Mean Squared Error (MSE) Loss Function is used to measure the average of the squares of the errors—that is, the average squared difference between the estimated values and the actual value. 
FORMULA: 
$L(\mathbf{w}) = \frac{1}{n} \sum_{i=1}^{n} (y_i - \mathbf{x}_i^\top \mathbf{w})^2$
ADDITIONAL:
The goal is to find the weights $\mathbf{w}$ that minimize this loss function.
PICTURE:
ID: 1717832387908
END

> [!question]- Analytical Solution for Linear Regression
TARGET DECK: Math::Machine Learning 0
START
Math_ONE_side
TITLE: Analytical Solution for Linear Regression
DESCRIPTION: 
The analytical solution for linear regression involves finding the weights that minimize the MSE loss function using the normal equation.
FORMULA: 
$\mathbf{w} = (\mathbf{X}^\top \mathbf{X})^{-1} \mathbf{X}^\top \mathbf{y}$
ADDITIONAL:
Where $\mathbf{X}$ is the matrix of input features, $\mathbf{y}$ is the vector of target values, and $\mathbf{w}$ is the vector of weights.
PICTURE:
ID: 1717832387913
END

> [!question]- Gauss-Markov Theorem
TARGET DECK: Math::Machine Learning 0
START
Math_TWO_side
TITLE: Gauss-Markov Theorem
DESCRIPTION: 
The Gauss-Markov theorem states that in a linear regression model where the errors have expectation zero and are uncorrelated and have equal variances, the best linear unbiased estimator (BLUE) of the coefficients is given by the ordinary least squares (OLS) estimator.
FORMULA: 
$\hat{\mathbf{w}} = (\mathbf{X}^\top \mathbf{X})^{-1} \mathbf{X}^\top \mathbf{y}$
ADDITIONAL:
This theorem assumes that the model is linear in parameters, there is no perfect multicollinearity, and the error terms have constant variance (homoscedasticity).
PICTURE:
ID: 1717832387918
END

> [!question]- Gradient Approach in Linear Regression
TARGET DECK: Math::Machine Learning 0
START
Math_ONE_side
TITLE: Gradient Approach in Linear Regression
DESCRIPTION: 
The gradient approach involves using gradient descent to iteratively update the weights to minimize the MSE loss function.
FORMULA: 
$\mathbf{w} := \mathbf{w} - \alpha \nabla L(\mathbf{w})$
ADDITIONAL:
Where $\alpha$ is the learning rate and $\nabla L(\mathbf{w}) = -\frac{2}{n} \mathbf{X}^\top (\mathbf{y} - \mathbf{X}\mathbf{w})$ is the gradient of the loss function with respect to the weights.
PICTURE:
ID: 1717832387922
END




#### 9. Multiclass classification. One-vs-one, one-vs-all, their properties.

> [!question]- Multiclass Classification: One-vs-One and One-vs-All Methods
TARGET DECK: Math::Machine Learning 0
START
Math_ONE_side
TITLE: Multiclass Classification: One-vs-One and One-vs-All Methods
DESCRIPTION: 
Multiclass classification involves classifying instances into one of three or more classes. Two popular strategies are One-vs-One (OvO) and One-vs-All (OvA).

One-vs-One (OvO): This method involves training a classifier for every possible pair of classes. For n classes, it trains $\frac{n(n-1)}{2}$ classifiers.

One-vs-All (OvA): This method involves training a single classifier per class, with the samples of that class as positive samples and all other samples as negative. For n classes, it trains n classifiers.
FORMULA: 
None
ADDITIONAL:
Example for OvO: For classes A, B, and C, train classifiers: A vs B, A vs C, B vs C.
Example for OvA: For classes A, B, and C, train classifiers: A vs (B and C), B vs (A and C), C vs (A and B).
PICTURE:
ID: 1717832873670
END

> [!question]- Properties of One-vs-One and One-vs-All Methods
TARGET DECK: Math::Machine Learning 0
START
Math_ONE_side
TITLE: Properties of One-vs-One and One-vs-All Methods
DESCRIPTION: 
Properties of One-vs-One (OvO):
- Requires $\frac{n(n-1)}{2}$ classifiers.
- Each classifier is trained on a smaller subset of the data.
- Can be computationally expensive for large n.
- Can handle imbalanced datasets better as each classifier deals with only two classes.

Properties of One-vs-All (OvA):
- Requires n classifiers.
- Each classifier is trained on the entire dataset.
- Simpler and less computationally expensive compared to OvO.
- Can be less effective for imbalanced datasets as each classifier is exposed to all classes.
FORMULA: 
None
ADDITIONAL:
Choosing between these methods often depends on the dataset size, class imbalance, and computational resources.
PICTURE:
ID: 1717832814543
END

> [!question]- One-vs-One Method and Properties
TARGET DECK: Math::Machine Learning 0
START
Math_ONE_side
TITLE: One-vs-One Method and Properties
DESCRIPTION: 
One-vs-One (OvO) method involves training a classifier for every possible pair of classes. For n classes, it trains $\frac{n(n-1)}{2}$ classifiers.

Properties of One-vs-One (OvO):
- Requires $\frac{n(n-1)}{2}$ classifiers.
- Each classifier is trained on a smaller subset of the data.
- Can be computationally expensive for large n.
- Can handle imbalanced datasets better as each classifier deals with only two classes.
FORMULA: 
None
ADDITIONAL:
Example for OvO: For classes A, B, and C, train classifiers: A vs B, A vs C, B vs C.
PICTURE:
ID: 1717832814547
END

> [!question]- One-vs-All Method and Properties
TARGET DECK: Math::Machine Learning 0
START
Math_ONE_side
TITLE: One-vs-All Method and Properties
DESCRIPTION: 
One-vs-All (OvA) method involves training a single classifier per class, with the samples of that class as positive samples and all other samples as negative. For n classes, it trains n classifiers.

Properties of One-vs-All (OvA):
- Requires n classifiers.
- Each classifier is trained on the entire dataset.
- Simpler and less computationally expensive compared to OvO.
- Can be less effective for imbalanced datasets as each classifier is exposed to all classes.
FORMULA: 
None
ADDITIONAL:
Example for OvA: For classes A, B, and C, train classifiers: A vs (B and C), B vs (A and C), C vs (A and B).
Choosing between these methods often depends on the dataset size, class imbalance, and computational resources.
PICTURE:
ID: 1717832814555
END


#### 12. Train, validation and test stages of model development. Overfitting problem, ways to detect it.

> [!question]- Train, Validation, and Test Stages
TARGET DECK: Math::Machine Learning 0
START
Math_ONE_side
TITLE: Train, Validation, and Test Stages
DESCRIPTION: 
In machine learning, data is typically split into three sets: training, validation, and test sets. 
- The training set is used to fit the model.
- The validation set is used to tune hyperparameters and select the best model.
- The test set is used to evaluate the model's performance on unseen data.
FORMULA: 
No specific formula.
ADDITIONAL:
The training set is usually the largest portion of data. The validation set helps in avoiding overfitting by tuning the model based on performance on this unseen set. The test set should only be used once the model is finalized to provide an unbiased evaluation of the model’s performance.
PICTURE:
ID: 1717833030121
END

> [!question]- Overfitting Problem
TARGET DECK: Math::Machine Learning 0
START
Math_ONE_side
TITLE: Overfitting Problem
DESCRIPTION: 
Overfitting occurs when a model learns the noise in the training data instead of the actual underlying pattern. This results in excellent performance on the training data but poor performance on unseen data.
FORMULA: 
No specific formula.
ADDITIONAL:
Overfitting can be detected by comparing the model’s performance on the training and validation sets. A significant gap between the training and validation performance indicates overfitting. Regularization techniques, such as L1 and L2 regularization, and methods like cross-validation can help mitigate overfitting.
PICTURE:
ID: 1717833030126
END

> [!question]- Ways to Detect Overfitting
TARGET DECK: Math::Machine Learning 0
START
Math_ONE_side
TITLE: Ways to Detect Overfitting
DESCRIPTION: 
Overfitting can be detected through several methods:
1. Cross-validation: Split the data into multiple folds and validate the model across these folds.
2. Learning curves: Plot training and validation error curves. If the training error is significantly lower than the validation error, overfitting is likely occurring.
3. Validation set performance: A large discrepancy between training and validation performance indicates overfitting.
FORMULA: 
No specific formula.
ADDITIONAL:
Techniques to prevent overfitting include using simpler models, increasing training data, using regularization methods (such as L1 and L2), and applying dropout in neural networks.
PICTURE:
ID: 1717832968746
END



#### 15. Decision tree construction procedure.

> [!question]- Decision Tree Definition
TARGET DECK: Math::Machine Learning 0
START
Math_TWO_side
TITLE: Decision Tree Definition
DESCRIPTION: 
is a non-parametric supervised learning algorithm used for classification and regression tasks. It builds a model in the form of a tree structure, where each internal node represents a feature (or attribute), each branch represents a decision rule, and each leaf node represents the outcome.
FORMULA: 
ADDITIONAL:
Easy to interpret and visualize. They can handle both numerical and categorical data and are prone to overfitting.
PICTURE:
ID: 1717833149993
END

> [!question]- Decision Tree Construction Procedure
TARGET DECK: Math::Machine Learning 0
START
Math_ONE_side
TITLE: Decision Tree Construction Procedure
DESCRIPTION: 
1. Select the best feature to split the data using a metric like Gini impurity or information gain.
2. Create a decision node based on this feature.
3. Partition the dataset into subsets based on the feature split.
4. Repeat the process recursively for each subset, treating each subset as a new dataset.
5. Stop the recursion when all data points in a subset belong to the same class, or when the maximum depth is reached.
FORMULA: 
Common metrics:
- Gini Impurity: $G = 1 - \sum_{i=1}^{C} p_i^2$
- Information Gain: $IG = H(parent) - \sum_{k \in children} \frac{n_k}{n_{parent}} H(k)$
ADDITIONAL:
The selection of the best split is crucial for the tree's performance. Pruning techniques can be applied post-construction to avoid overfitting.
PICTURE:
ID: 1717833149999
END



#### 18. Random Forest, Random subspace method.

> [!question]- Random Forest
TARGET DECK: Math::Machine Learning 0
START
Math_ONE_side
TITLE: Random Forest
DESCRIPTION: 
Random Forest is an ensemble learning method for classification, regression, and other tasks that operates by constructing multiple decision trees during training and outputting the mode of the classes (classification) or mean prediction (regression) of the individual trees.
FORMULA: 
N/A
ADDITIONAL:
Random Forests generally improve the performance of the model by reducing overfitting through averaging multiple decision trees' predictions. It also uses the technique of bootstrap aggregation (bagging) to construct multiple trees.
Example: 
Imagine you want to classify whether an email is spam or not. A Random Forest model will create multiple decision trees, each trained on different random subsets of the data and features. At prediction time, each tree votes for "spam" or "not spam," and the final prediction is based on the majority vote.
PICTURE:
ID: 1717833267859
END

> [!question]- Random Subspace Method
TARGET DECK: Math::Machine Learning 0
START
Math_ONE_side
TITLE: Random Subspace Method
DESCRIPTION: 
The Random Subspace Method involves training multiple classifiers on different random subsets of the feature space and combining their predictions. It's a way to introduce diversity into the ensemble by varying the feature subsets rather than the data samples.
FORMULA: 
N/A
ADDITIONAL:
This method helps in improving the model's robustness and accuracy by reducing the correlation between individual models. It is particularly useful in high-dimensional spaces where overfitting is a concern.
Example:
Consider a dataset with 100 features for predicting house prices. Using the Random Subspace Method, several models are trained, each on a random subset of, say, 20 features. Each model makes its prediction, and the final prediction is an average (in regression) or a majority vote (in classification) of all models' predictions.
PICTURE:
ID: 1717833267872
END



#### 21. Backpropagation, chain rule.
> [!question]- Backpropagation
TARGET DECK: Math::Machine Learning 0
START
Math_ONE_side
TITLE: Backpropagation
DESCRIPTION: 
Backpropagation is an algorithm used for training artificial neural networks. It calculates the gradient of the loss function with respect to the weights of the network by using the chain rule, propagating the error backward through the network layers.
FORMULA: 
$\delta^{(L)} = \nabla_a L \odot \sigma'(z^{(L)})$
$\delta^{(l)} = ((\mathbf{W}^{(l+1)})^\top \delta^{(l+1)}) \odot \sigma'(z^{(l)})$
ADDITIONAL:
- $\delta^{(L)}$ represents the error term for the output layer.
- $\delta^{(l)}$ represents the error term for layer $l$.
- $\sigma'(z)$ is the derivative of the activation function.
- This algorithm requires forward and backward passes through the network.
PICTURE:
ID: 1717833363020
END

> [!question]- Chain Rule in Backpropagation
TARGET DECK: Math::Machine Learning 0
START
Math_ONE_side
TITLE: Chain Rule in Backpropagation
DESCRIPTION: 
The chain rule is a mathematical principle used in calculus to compute the derivative of the composition of multiple functions. In backpropagation, it helps in calculating the gradient of the loss function with respect to each weight by propagating the error backward through each layer of the network.
FORMULA: 
$\frac{\partial L}{\partial w_{ij}^{(l)}} = \frac{\partial L}{\partial a_j^{(l)}} \cdot \frac{\partial a_j^{(l)}}{\partial z_j^{(l)}} \cdot \frac{\partial z_j^{(l)}}{\partial w_{ij}^{(l)}}$
ADDITIONAL:
- $L$ is the loss function.
- $a_j^{(l)}$ is the activation of neuron $j$ in layer $l$.
- $z_j^{(l)}$ is the input to neuron $j$ in layer $l$.
- $w_{ij}^{(l)}$ is the weight connecting neuron $i$ in layer $l-1$ to neuron $j$ in layer $l$.
PICTURE:
ID: 1717833363052
END



#### 24. Losses for NNs: logistic loss, cross-entropy.
> [!question]- Logistic Loss
TARGET DECK: Math::Machine Learning 0
START
Math_ONE_side
TITLE: Logistic Loss
DESCRIPTION: 
Logistic loss, also known as log-loss or binary cross-entropy loss, is used for binary classification problems. It measures the performance of a classification model whose output is a probability value between 0 and 1.
FORMULA: 
$L(y, \hat{y}) = - \left[ y \log(\hat{y}) + (1 - y) \log(1 - \hat{y}) \right]$
ADDITIONAL:
- $y$ is the true label (0 or 1).
- $\hat{y}$ is the predicted probability of the positive class.
- The logistic loss penalizes incorrect predictions more heavily the more confident the incorrect prediction is.
Example:
If $y = 1$ and $\hat{y} = 0.9$, then $L(1, 0.9) = - \left[ 1 \log(0.9) + 0 \log(0.1) \right] = - \log(0.9)$.
PICTURE:
ID: 1717833432682
END

> [!question]- Cross-Entropy Loss
TARGET DECK: Math::Machine Learning 0
START
Math_ONE_side
TITLE: Cross-Entropy Loss
DESCRIPTION: 
Cross-entropy loss is used for multi-class classification tasks. It measures the difference between two probability distributions: the true labels and the predicted probabilities.
FORMULA: 
$L(\mathbf{y}, \hat{\mathbf{y}}) = - \sum_{i=1}^{C} y_i \log(\hat{y}_i)$
ADDITIONAL:
- $C$ is the number of classes.
- $\mathbf{y}$ is a one-hot encoded vector of true labels.
- $\hat{\mathbf{y}}$ is the predicted probability distribution over the classes.
- Cross-entropy loss increases as the predicted probability diverges from the actual label.
Example:
For a three-class classification problem, if the true label is the second class, $\mathbf{y} = [0, 1, 0]$ and the predicted probabilities are $\hat{\mathbf{y}} = [0.1, 0.8, 0.1]$, then $L(\mathbf{y}, \hat{\mathbf{y}}) = - (0 \log(0.1) + 1 \log(0.8) + 0 \log(0.1)) = - \log(0.8)$.
PICTURE:
ID: 1717833432688
END


#### 27. Regularization in Deep Learning: Dropout, Batch Normalization. Differences in training and evaluation stages.
> [!question]- Regularization in Deep Learning
TARGET DECK: Math::Machine Learning 0
START
Math_TWO_side
TITLE: Regularization in Deep Learning
DESCRIPTION: 
Regularization techniques in deep learning are methods used to prevent overfitting by adding constraints to the model, promoting generalization over fitting to the training data.
ADDITIONAL:
- **Common Techniques**: 
  - **L1 and L2 Regularization**: Adds a penalty equal to the absolute value (L1) or square (L2) of the weights.
  - **Dropout**: Randomly drops neurons during training.
  - **Batch Normalization**: Normalizes inputs during training and uses learned parameters during evaluation.
- **Example**: L2 regularization adds $\lambda \sum w^2$ to the loss function, where $\lambda$ is the regularization parameter.
PICTURE:
ID: 1717833556717
END

> [!question]- Dropout Regularization
TARGET DECK: Math::Machine Learning 0
START
Math_TWO_side
TITLE: Dropout Regularization
DESCRIPTION: 
Dropout is a regularization technique where randomly selected neurons are ignored during training. This prevents overfitting by ensuring that the model does not rely too heavily on any individual neuron.
FORMULA: 
During training: $\mathbf{h} = \mathbf{h} \odot \mathbf{r}$ where $\mathbf{r} \sim \text{Bernoulli}(p)$
ADDITIONAL:
In the evaluation stage, no neurons are dropped, but the output is scaled by the dropout rate $p$. This ensures the expected value of the output is the same during training and evaluation. For example, if $p=0.5$, the output is scaled by $0.5$ during evaluation.
PICTURE:
ID: 1717833556722
END

> [!question]- Batch Normalization
TARGET DECK: Math::Machine Learning 0
START
Math_ONE_side
TITLE: Batch Normalization
DESCRIPTION: 
Batch normalization is a technique to improve the stability and performance of neural networks by normalizing the input of each layer.
ADDITIONAL:
- **Training Stage**: Normalizes each mini-batch and learns scale and shift parameters.
- **Evaluation Stage**: Uses the learned parameters to normalize the inputs.
- **Example**: A layer's activations are transformed to have zero mean and unit variance during training.
PICTURE:
ID: 1717833556726
END

> [!question]- Differences in Training and Evaluation Stages
TARGET DECK: Math::Machine Learning 0
START
Math_ONE_side
TITLE: Differences in Training and Evaluation Stages
DESCRIPTION: 
The key differences between training and evaluation stages in regularization techniques like Dropout and Batch Normalization.
ADDITIONAL:
- **Dropout**:
  - **Training**: Randomly drops neurons.
  - **Evaluation**: Uses all neurons.
- **Batch Normalization**:
  - **Training**: Normalizes mini-batches and learns parameters.
  - **Evaluation**: Uses learned parameters for normalization.
PICTURE:
ID: 1717833556731
END



#### 30. Matrix convolution. Convolutional layer, backpropagation through it. Hyperparameters of Convs. 1x1 convolutions, comparison to FC layers. Max/Average Pooling.

> [!question]- Matrix Convolution
TARGET DECK: Math::Machine Learning 0
START
Math_ONE_side
TITLE: Matrix Convolution
DESCRIPTION: 
Matrix convolution is a mathematical operation used in signal processing and image processing where an input matrix (or image) is combined with a filter (or kernel) to produce a transformed matrix. Convolutional operations are fundamental in Convolutional Neural Networks (CNNs) for feature extraction.
FORMULA: 
$(f * g)(t) = \int_{-\infty}^{\infty} f(\tau)g(t-\tau) d\tau$
ADDITIONAL:
In discrete form, convolution is represented as: $(f * g)[n] = \sum_{m=-\infty}^{\infty} f[m] g[n - m]$. 
Example: For a 3x3 kernel applied to an image, each output pixel is the sum of element-wise multiplications of the kernel and the corresponding region of the input image.
PICTURE:
ID: 1717833618928
END

> [!question]- Convolutional Layer and Backpropagation
TARGET DECK: Math::Machine Learning 0
START
Math_ONE_side
TITLE: Convolutional Layer and Backpropagation
DESCRIPTION: 
A convolutional layer applies a set of filters to the input to produce feature maps. During backpropagation, gradients are computed for the filters and input feature maps to update the weights.
FORMULA: 
$\frac{\partial L}{\partial \mathbf{X}} = \mathbf{K}^\top * \frac{\partial L}{\partial \mathbf{Y}}$
ADDITIONAL:
Where $\mathbf{X}$ is the input, $\mathbf{K}$ is the filter, $\mathbf{Y}$ is the output, and $L$ is the loss function.
Example: If the output gradient $\frac{\partial L}{\partial \mathbf{Y}}$ is known, the gradient with respect to the input $\mathbf{X}$ can be computed by convolving $\frac{\partial L}{\partial \mathbf{Y}}$ with the transposed filter $\mathbf{K}^\top$.
PICTURE:
ID: 1717833618934
END

> [!question]- Hyperparameters of Convolutional Layers
TARGET DECK: Math::Machine Learning 0
START
Math_ONE_side
TITLE: Hyperparameters of Convolutional Layers
DESCRIPTION: 
Hyperparameters in convolutional layers include the size and number of filters, stride, padding, and dilation.
FORMULA: 
N/A
ADDITIONAL:
- **Filter Size**: Determines the dimensions of the filter/kernel.
- **Number of Filters**: Determines the depth of the output feature maps.
- **Stride**: The step size with which the filter moves across the input.
- **Padding**: Adding extra pixels around the input to control the spatial dimensions of the output.
- **Dilation**: Expands the filter by inserting spaces between the elements.
PICTURE:
ID: 1717833618937
END

> [!question]- 1x1 Convolutions vs Fully Connected Layers
TARGET DECK: Math::Machine Learning 0
START
Math_ONE_side
TITLE: 1x1 Convolutions vs Fully Connected Layers
DESCRIPTION: 
1x1 convolutions apply a single weight and bias to each pixel, transforming the input depth without affecting spatial dimensions. Fully connected (FC) layers connect every input neuron to every output neuron.
FORMULA: 
N/A
ADDITIONAL:
- **1x1 Convolutions**: Useful for dimensionality reduction and increasing non-linearity.
- **Fully Connected Layers**: Typically used at the end of CNN architectures for classification tasks.
Example: In a CNN, 1x1 convolutions can reduce the number of channels while preserving spatial information, unlike FC layers which flatten the input.
PICTURE:
ID: 1717833618941
END

> [!question]- Max Pooling vs Average Pooling
TARGET DECK: Math::Machine Learning 0
START
Math_ONE_side
TITLE: Max Pooling vs Average Pooling
DESCRIPTION: 
Pooling layers reduce the spatial dimensions of the input by summarizing regions of the input feature maps. Max pooling selects the maximum value, while average pooling computes the average value.
FORMULA: 
N/A
ADDITIONAL:
- **Max Pooling**: Extracts the most prominent features by selecting the maximum value within each region.
- **Average Pooling**: Computes the mean of the values within each region, providing a smoother approximation.
Example: Max pooling with a 2x2 window and stride 2 reduces the input dimensions by half, selecting the maximum value in each 2x2 region.
PICTURE:
ID: 1717833618945
END



