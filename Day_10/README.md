# Regularization

## Topics covered in today's module
* L1/L2 Regularization
* Dropout
* Overfitting
* Underfitting

## Main takeaways from doing today's assignment
In L1 regularization, the penalty term is the absolute value of the weights, which forces the model to shrink some of the weights to zero, resulting in sparse models. This can be helpful for feature selection, as it identifies which features are most important.

In L2 regularization, the penalty term is the square of the weights, which encourages the model to use smaller weights overall, but doesn't necessarily force any to zero. This can help to smooth out the learned function and prevent overfitting.

By adding a penalty to the loss function, L1 and L2 regularization prevent the model from simply memorizing the training data and instead encourage it to learn more generalizable patterns. This can result in better performance on new, unseen data.

Dropout, on the other hand, works by randomly dropping out some of the neurons during training, which can help to prevent overfitting by reducing the model's reliance on any single feature or combination of features. Dropout can be particularly effective when used in conjunction with L2 regularization, as it can help to prevent the model from relying too heavily on any individual feature, even those with very small weights.

## Challenging, interesting, or exciting aspects of today's assignment
Understanding why adding both L2 regularization and Dropout

It can make sense to add both L2 regularization and Dropout when training a neural network to help prevent overfitting. L2 regularization adds a penalty term to the loss function based on the magnitude of the weights, encouraging smaller weights and simpler models. Dropout randomly drops out a fraction of the neurons during training, forcing the network to learn more robust representations that are not dependent on any one particular neuron.

Together, L2 regularization and Dropout can complement each other by encouraging both smaller weights and more diverse representations. L2 regularization will encourage the network to use fewer and smaller weights, while Dropout will encourage the network to use more diverse and robust representations. However, it is important to tune the regularization strengths and dropout rates carefully to avoid underfitting or overfitting.

## Additional resources used 
https://towardsdatascience.com/regularization-dropout-in-deep-learning-5198c2bf6107
