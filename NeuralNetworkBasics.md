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

*Figure from The Elements of Statistical Learning by Hastie et al*

## Feedforward neural network

With perceptron as a building block, a neural network has **multiple layers that have multiple neurons**. In the feedforward architecture, the connections are strictly from one layer to the next; there are no "loops." To obtain the neural network output, the input vector is passed through all the layers (forward propagation/pass).

<img src="/figures/neuralnet.png" width="40%">

*Figure from Wikipedia*

## Exercise 1

> Implement a neural network layer. Hint: look at neuron and use matrix multiplication.

## Exercise 2

> Implement a forward pass through multiple layers. Hint: keep track of the current vector and use layer.

## Loss function

The loss (cost) function *L* evaluates model performance by comparing *y_pred* against *y_true*. Since *y_pred* is a function of model parameters (weights and biases), we can imagine a loss landscape of *L(y_pred, y_true)* with respect to model parameters. 

<img src="/figures/landscape.png" width="60%">

*Figure from Visualizing the Loss Landscape of Neural Nets by Li et al*

## Gradient descent

Hence training a neural network is an optimization problem: finding the optimal parameters to minimize the loss function. The gradient descent algorithm attempts to find the minimum in the loss landscape by following the gradient (downward slope).

<img src="/figures/descent.png" width="40%">

*Figure from Wikipedia*

## Back-propagation

The back-propagation algorithm calculates the gradient with chain rule recursively. 

<img src="/figures/chainrule.png" width="80%">

*Figure from Wikipedia*

## Computational graph

A computational graph represents a complex function through basic operations on a graph; it allows for automatic differentiation in Tensorflow, making back-propagation straightforward.

<img src="/figures/graph.png" width="60%">

*Figure from Deep Learning by Goodfellow et al*


## Exercise 3

> Implement gradient descent in Tensorflow.

## References

Tensorflow documentation https://www.tensorflow.org/versions/master/programmers_guide/low_level_intro

Chapter of Deep Learning book http://www.deeplearningbook.org/contents/mlp.html

Blog post on back-propagation http://colah.github.io/posts/2015-08-Backprop/
