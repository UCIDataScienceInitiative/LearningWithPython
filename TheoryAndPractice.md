## Theory of neural networks

Deeper neural networks have more expressive power.

<img src="/figures/power.png" width="60%">

*Figure from Bayesian Methods for Machine Learning by Radford M. Neal*

Moreover, it has been shown that neural networks are universal approximators.

<img src="/figures/universal.png" width="100%">

*Figure from Wikipedia*

<img src="/figures/deeper.png" width="40%">

*Meme from the interwebs*

## Overfitting and regularization

However, deeper neural networks face the problem of overfitting.

<img src="/figures/overfitting.png" width="60%">

*Figure from Deep Learning by Goodfellow et al*

One way to prevent overfitting is by adding a weight penalty to the loss function. The weight penalty is usually in the form of L1 or L2 norm. One can think about weight penalty from the perspective of variable selection in regression. 

<img src="/figures/lasso.png" width="60%">

*Figure from The Elements of Statistical Learning by Hastie et al*

Another simple way to prevent overfitting is dropout. Dropout randomly removes neurons or connections in the network during training. There are many interpretations of dropout from "robust" representation to Bayesian inference.

<img src="/figures/dropout.png" width="60%">

*Figure from Dropout: A Simple Way to Prevent Neural Networks from Overfitting by Srivastava et al*

## Local minima and stochastic gradient descent

Gradient descent is a first-order "local" algorithm and can be trapped in local minima. Stochastic gradient descent only uses a batch of the data at a time and can be combined with "tricks" such as momentum and learning rate decay. Training neural networks involve tuning various hyperparameters:

* weight penalty, dropout probability
* learning rate or step size
* batch size
* momentum, learning rate schedule...

<img src="/figures/local.png" width="60%">

*Figure from Deep Learning by Goodfellow et al*

## Other issues

* Vanishing gradient and ReLU
* Data pre-processing

## Mini project

> Build a neural network in Tensorflow to predict player position with FIFA data. 

> Plot loss curves to detect overfitting and apply appropriate regularization.

> Explore the effects of hyperparameters and find the "best" combination.

## References

A visual proof that neural nets can compute any function http://neuralnetworksanddeeplearning.com/chap4.html

Why momentum really works https://distill.pub/2017/momentum/

What my deep model doesn't know http://mlg.eng.cam.ac.uk/yarin/blog_3d801aa532c1ce.html
