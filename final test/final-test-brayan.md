# Machine Learning for Masters Final Test - Second Variant

## Name: Brayan Duran Medina

### Question for all students: Supervised learning problem statement. Regression and classification problems. What’s the difference?

#### Supervised Supervised learning problem statement:

Let's denote:

-   Training set $\{(x^{(i)}, y^{(i)})\}_{i=1}^{n}$ ,where

    -   $x^{(i)} \in \mathbb{R}^p, y^{(i)} \in \mathbb{R}$ for regression
    -   $x^{(i)} \in \mathbb{R}^p, y^{(i)} \in \{C_1, \ldots, C_K\}$ for classification

-   Model $f(x)$ predicts some value for every object
-   Loss function $L(x, y, f)$ that should be minimized

#### Diference between regression and classification problems:

The main difference between regression and classification problems is the type of output variable that we are trying to predict. In regression problems, the output variable is a continuous value, while in classification problems, the output variable is a discrete value.

### 2. What is the gradient? How is it used in optimization?

The gradient is a vector that points in the direction of the greatest increase of a function. It is used in optimization to find the minimum of a function. The gradient is used to update the parameters of a model in the direction of the greatest decrease of the loss function.

### 4. What is validation? Cross validation?

Validation is a technique used to evaluate the performance of a model. It is used to estimate how well a model will perform on new data. Cross validation is a technique used to evaluate the performance of a model by splitting the data into k folds and training the model k times, each time using a different fold as the validation set.

### 6. What are precision and recall metrics?

Precision is the ratio of true positive predictions to the sum of true positive and false positive predictions. Recall is the ratio of true positive predictions to the sum of true positive and false negative predictions.

### 8. How are parameters different from hyperparameters? E.g. what are parameters in linear models and decision trees? Hyperparameters?

Parameters are the values that a model learns from the data. They are the weights in a linear model and the split points in a decision tree. Hyperparameters are the values that are set before the model is trained. They are for example the learning rate in a linear model and the maximum depth in a decision tree, etc.

### 10. What is backpropagation? How does it work? E.g. how would gradient propagate through a linear layer? Through ReLU?

Backpropagation is a technique used to calculate the gradients of the loss function with respect to the parameters of a model. It works by using the chain rule to calculate the gradients of the loss function with respect to the parameters of the model layer by layer. The gradients are then used to update the parameters of the model.

The gradient of a linear layer is the input to the layer transposed and multiplied by the gradient of the loss function with respect to the output of the layer.

### 12. What is dropout? How does it work in a neural network? Does it change its behaviour on the inference (test) stage?

Dropout is a regularization technique used to prevent overfitting in neural networks. It works by randomly setting a fraction of the input units to 0 at each update during training. This forces the network to learn a more robust representation of the data. During the inference stage, the dropout is turned off and the weights are scaled by the dropout rate.

### 14. How does RNN work? Can you combine CNN and RNN somehow?

RNN stands for Recurrent Neural Network. It is a type of neural network that is designed to work with sequences of data. It works by processing the input data one element at a time and maintaining a hidden state that captures information about the sequence. CNN and RNN can be combined by using the output of a CNN as the input to an RNN. This is useful when working with sequences of images.
