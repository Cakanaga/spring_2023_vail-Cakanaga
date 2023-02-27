# Optimization

## Topics covered in today's module
* Optimization
* Gradident Descent
* Optimizers(SGD, ADAM, etc.)

## Main takeaways from doing today's assignment

Optimize = minimize loss function

Optimizers and loss functions are both crucial components of the training process in machine learning. The loss function is used to measure the difference between the predicted output of a model and the true output, while the optimizer is used to adjust the model's parameters to minimize the loss.

There are many problems that do not require optimization such as Linear Regression

Other different ways we can optimize:
* Stochastic Gradient Descent (SGD): SGD is a variant of gradient descent where instead of computing the gradient over the entire dataset, the gradient is computed on a small random subset of the data. This makes it more efficient and effective for large datasets.

* Adam: Adam is an optimization algorithm that uses a combination of adaptive gradient methods and momentum-based methods. It is designed to converge faster and more efficiently than other optimization methods, especially for large-scale deep learning problems.

* Adagrad: Adagrad is an adaptive learning rate optimization algorithm that adjusts the learning rate for each parameter based on its historical gradients. It is particularly useful in deep learning applications with sparse data.

## Challenging, interesting, or exciting aspects of today's assignment
Implementing the AdaGrad optimizer and plotting a loss/epochs curve similar to our previous plot was a little challenging

## Additional resources used 
https://towardsdatascience.com/deep-learning-optimizers-436171c9e23f
