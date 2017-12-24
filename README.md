# multi_layer_perceptron
This project involves the implementation of efficient and effective MLP (multi-layer perceptron) on MNIST data set. The MNIST data comprises of digital images of several digits ranging from 0 to 9. Each image is 28 x 28 pixels. Thus, the data set has 10 levels of classes.

MLP is a supervised machine learning algorithm for regression or classification. Within the input and output, there might be some nonlinear layers, called hidden layers. Hence, MLP has the ability to learn nonlinear models. Each of the hidden layers comprises of neurons, which is the number of nodes in the hidden layer. MLP is sensitive to unscaled features, thus it might be important to scale the feature - [0, 1], hence the training and testing sets will be divided by 255.

Regularization in MLP:
MLPClassifier in sklearn uses parameter alpha for regularization (L2 regularization) [1]. Alpha is used for penalizing the weights, hence, ensuring that the weights are as small as possible. GridsearchCV can be used to obtain the best value of alpha, values ranging from 1e-6 to 1e-1 (log scale) are mostly used.

Solver in MLP:
In Sklearn, the solver for weight optimization could be any of 'lbfgs', 'sgd', or 'adam' [2]. SGD refers to stochastic gradient descent, it performs better than the other two.
