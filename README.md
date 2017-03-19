# DeepLearning

## ConvolutionalNeuralNetwork
Apply convolutional neural network to classify images from the CIFAR-10 dataset, which includes 10 labels -- airplane, automobile, bird, cat, deer, dog, frog, horse, ship and truck:
* preprocess data by normalizing pixel features, one-hot encoding labels, randomizing the order of samples
* implemented functions of convolution and max pooling layer (same padding for both filter and max pooling, ReLU as non-linear activation function), flatten layer (to change image data from 4-D tensor to 2-D tensor), fully-connected layer (ReLU as non-linear activation function), and output layer, using Tensorflow Neural Network API
* construct convolutional neural network model that includes 2 convolution and max pooling layers (40 outputs, 5-by-5 filter with 1-by-1 strides, 2-by-2 max pooling with 2-by-2 strides; followed by 100 outputs, 5-by-5 filter with 1-by-1 strides, 2-by-2 max pooling with 2-by-2 strides) and 1 fully connected layer (6400 outputs with a dropout rate to be tuned)
* tune the value of hyperparameters (30 epochs, 256 batch size, and a rate of 0.75 to keep a node using dropout)
* achieve over 63% accuracy for all 5 training batches and 62.9% for the test batch (whereas random guessing would give one 10% accuracy)
