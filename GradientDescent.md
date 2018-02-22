## Loss function


The loss (cost) function *L* evaluates model performance by comparing *y_pred* against *y_true*. Since *y_pred* is a function of model parameters *Theta* (weights and biases), we can imagine a loss landscape of *L(y_pred, y_true)* with respect to *Theta*. The loss landscape shows values of *L* at different positions in the parameter space (combinations of different weights and biases). 

<img src="/figures/landscape.png" width="60%">

## Gradient descent

Training a neural network is an optimization problem: finding the optimal parameters to minimize the loss function. The gradient descent algorithm attempts to find the minimum in the loss landscape by following the gradient (downward slope).

<img src="/figures/descent.png" width="40%">

## Backpropagation

The backpropagation algorithm calculates the gradient with chain rule and trains a neural network iteratively. 

<img src="/figures/chainrule.png" width="60%">

## Computational graph

A computational graph allows for automatic differentiation in Tensorflow, making backpropagation straightforward.

<img src="/figures/graph.png" width="60%">

