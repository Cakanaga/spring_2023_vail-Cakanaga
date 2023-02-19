# Classification Loss Functions

## Topics covered in today's module
* Kullback Leibler Divergence Loss
* Binary Cross-Entropy
* Categorical Cross-Entropy
* Sparse Categorical Cross-Entropy

## Main takeaways from doing today's assignment

# Multi-class vs. Multi-label Classification problem
In a multi-class classification problem, each data point can belong to only one class out of a set of mutually exclusive classes. For example, a handwritten digit classification problem, where each image is assigned to one of the 10 digits (0-9), is a multi-class classification problem.

On the other hand, in a multi-label classification problem, each data point can belong to one or more classes out of a set of non-mutually exclusive classes. For example, an image classification problem where each image can have multiple objects present in it is a multi-label classification problem.

To learn a multi-class classification problem, we typically use a softmax activation function in the output layer of the neural network, and the cross-entropy loss function, such as categorical cross-entropy, is used to train the model.

To learn a multi-label classification problem, we typically use a sigmoid activation function in the output layer of the neural network, and the binary cross-entropy loss function is used to train the model. In this case, the output layer of the neural network has one node per label, and the sigmoid activation function is used to output the probability that the input belongs to each label.

# Binary Cross entropy vs Categorical Cross entropy
Binary cross entropy is used for binary classification problems, where there are only two classes. It calculates the difference between the predicted probabilities of the positive class and the true labels of the positive class. It can be thought of as a special case of categorical cross entropy with only two classes.

Categorical cross entropy, on the other hand, is used for multi-class classification problems, where there are more than two classes. It calculates the difference between the predicted probabilities of all classes and the true labels. In this case, each class is treated as an independent binary classification problem, and the total loss is the average of the binary cross entropy for each class.

Mathematically, both binary cross entropy and categorical cross entropy are forms of cross-entropy loss, which measures the distance between two probability distributions. However, categorical cross entropy is more general, as it can handle any number of classes, while binary cross entropy is a special case of categorical cross entropy with only two classes.

# Sparse Cross entropy and Categorical Cross entropy
The difference between them lies in the way the labels are represented.

Categorical cross entropy is used when the labels are one-hot encoded, meaning that each label is represented as a vector with a 1 in the position of the true class and 0s everywhere else. The predicted probabilities are also represented as vectors of the same length.

Sparse categorical cross entropy is used when the labels are integers representing the class indices. In other words, the true label for each example is represented as a single integer indicating the index of the correct class. The predicted probabilities are still represented as vectors, but they have a length equal to the number of classes.

In terms of the calculation of the loss, the two loss functions are essentially the same. The difference is that sparse categorical cross entropy is more efficient when the labels are represented as integers, because it avoids the computation required to convert the integer labels to one-hot encoded labels.

## Challenging, interesting, or exciting aspects of today's assignment
An exciting part was creating the function for categorical cross entropy

## Additional resources used 
https://cwiki.apache.org/confluence/display/MXNET/Multi-hot+Sparse+Categorical+Cross-entropy#:~:text=The%20only%20difference%20between%20sparse,only%20belong%20to%20one%20class.
 https://stats.stackexchange.com/questions/260505/should-i-use-a-categorical-cross-entropy-or-binary-cross-entropy-loss-for-binary
