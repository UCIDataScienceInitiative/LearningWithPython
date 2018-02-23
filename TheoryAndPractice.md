## Theory of neural networks

Deeper neural networks have more expressive power.

<img src="/figures/power.png" width="60%">

*Figure from Bayesian Methods for Machine Learning by Radford M. Neal*

Moreover, it has been shown that neural networks are universal approximators.

<img src="/figures/universal.png" width="80%">

*Figure from Wikipedia*

<img src="/figures/deeper.png" width="40%">

*Meme from the interwebs*

## Overfitting and regularization

However, deeper neural networks face the problem of overfitting.

<img src="/figures/overfitting.png" width="60%">

*Figure from Deep Learning by Goodfellow et al*

One way to prevent overfitting is by adding a weight penalty to the loss function. The weight penalty is usually in the form of L1 or L2 norm. The amount of weight penalty to add is a hyperparameter that needs to be tuned. One can think about weight penalty from the perspective of variable selection in regression.

<img src="/figures/lasso.png" width="60%">

*Figure from The Elements of Statistical Learning by Hastie et al*

Another simple way to prevent overfitting is dropout. There are many interpretations of dropout from "robust" representation to Bayesian inference.

<img src="/figures/dropout.png" width="60%">

*Figure from Dropout: A Simple Way to Prevent Neural Networks from Overfitting by Srivastava et al*

## Local minima and stochastic gradient descent

<img src="/figures/local.png" width="60%">

*Figure from Deep Learning by Goodfellow et al*

## Other issues

* Vanishing gradient and ReLU
* Data pre-processing

## Mini project

> Build a neural network in Tensorflow to predict player position using with FIFA data. 

> Plot loss curves to detect overfitting and apply appropriate regularization.

> Explore the effects of hyperparameters and find the "best" combination.
