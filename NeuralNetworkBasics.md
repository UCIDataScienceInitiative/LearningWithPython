## Perceptron

The perceptron models a single neuron. 

* Input vector
* Weights and bias
* Activation function

<img src="/figures/perceptron.png" width="50%">

*Figure from Wikipedia*

There are different activation functions. Most of them map the input to between 0 and 1, where 0 means the neuron is inactive and 1 means the neuron is excited.

<img src="/figures/activation.png" width="60%">

*Figure from The Elements of Statistical Learning by Hastie et al*

## Exercise 0

> Implement sigmoid activation.

A perceptron with sigmoid activation is essentially logistic regression, a generalized linear model. It is considered linear because the decision boundary is a line.

<img src="/figures/logistic.png" width="60%">

## Feedforward neural network

With perceptron as a building block, a neural network has multiple layers that have multiple neurons. In a feedforward neural network, the connections are strictly from one layer to the next; there are no loops. Neural networks with loops are called recurrent neural networks (RNN). 

<img src="/figures/neuralnet.png" width="40%">

## Exercise 1

> Implement a neural network layer. Hint: use neuron and matrix multiplication is helpful.

## Exercise 2

> Implement a forward pass through multiple layers. Hint: keep track of the current vector and use layer.

## Loss function

The loss (cost) function *L* evaluates model performance by comparing *y_pred* against *y_true*. Since *y_pred* is a function of model parameters *Theta* (weights and biases), we can imagine a loss landscape of *L(y_pred, y_true)* with respect to *Theta*. The loss landscape shows values of *L* at different positions in the parameter space (combinations of different weights and biases). 

<img src="/figures/landscape.png" width="60%">

## Gradient descent

Training a neural network is an optimization problem: finding the optimal parameters to minimize the loss function. The gradient descent algorithm attempts to find the minimum in the loss landscape by following the gradient (downward slope).

<img src="/figures/descent.png" width="40%">

## Backpropagation

The backpropagation algorithm calculates the gradient with chain rule and trains a neural network iteratively. 

<img src="/figures/chainrule.png" width="80%">

## Computational graph

A computational graph allows for automatic differentiation in Tensorflow, making backpropagation straightforward.

<img src="/figures/graph.png" width="60%">

## Exercise 3

> Implement gradient descent in Tensorflow.
