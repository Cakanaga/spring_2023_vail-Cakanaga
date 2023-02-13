# Deep Learning and TensorFlow

## Topics covered in today's module
* Linear models in machine learning
* Introduction to TensorFlow
* Dataloaders
* Building a simple Neural Network

## Main takeaways from doing today's assignment
The lower the loss, the better a model (unless the model has over-fitted to the training data). The loss is calculated on training and validation and its interperation is how well the model is doing for these two sets. Unlike accuracy, loss is not a percentage. It is a summation of the errors made for each example in training or validation sets.

Loss value implies how well or poorly a certain model behaves after each iteration of optimization. Ideally, one would expect the reduction of loss after each, or several, iteration(s).

## Challenging, interesting, or exciting aspects of today's assignment
Understanding how and why we scale data to 0,1

We scales these values to a range of 0 and 1 because activation functions used in neural networks are usually sigmoidal in nature, which means that inputs outside the range of 0 to 1 can saturate the activation function. This can lead to slow convergence or even non-convergence of the model during training. Scaling the values to the 0-1 range helps to avoid these issues and speeds up convergence.

If the pixel values were not scaled, the model might have trouble learning patterns in the data. This is because the weights of the model would have to be adjusted over a much larger range of values, which can slow down convergence.

## Additional resources used 
https://medium.com/arteos-ai/the-differences-between-sigmoid-and-softmax-activation-function-12adee8cf322
