# Artificial Neural Networks

## Topics covered in today's module
* Introduction to Neural Networks
* Hyperparameters
* Forward Pass
* Backpropagation
* Computing accuracy

## Main takeaways from doing today's assignment

Hyperparameters are attributes, whose values control the learning process and determine the values of model parameters that a learning algorithm ends up learning. The prefix ‘hyper_’ suggests that they are ‘top-level’ parameters that control the learning process and the model parameters that result from it.

We initialize with random weights because it keeps the weights away from the regions where they might vanish or 'explode'

The forward pass computes the output of the network given an input, while the backward pass computes the gradients of the loss with respect to the network parameters and updates the network parameters accordingly.

## Challenging, interesting, or exciting aspects of today's assignment
Now, if we wanted the output  y  to be a vector of size 4, and the input  x  to be a vector of size 2: a) what should the dimensions of W be? b) should we initialize the weights as np.random.randn(dimension of current layer, dimension of its previous layer), or should we instead use np.random.randn(dimension of the previous layer, dimension of current layer)?

## Additional resources used 
https://machinelearningmastery.com/why-initialize-a-neural-network-with-random-weights/
