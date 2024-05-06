# Convolutional Neural Network (CNN) for Image Classification

This project involves implementing a Convolutional Neural Network (CNN) for an image classification task. The CNN architecture consists of six basic components:

1. **Convolution Layer**: This layer has four hyperparameters: the number of output channels, filter dimension, stride, and padding.
2. **Activation Layer**: An element-wise Rectified Linear Unit (ReLU) activation function.
3. **Max-Pooling Layer**: This layer has two parameters: filter dimension and stride.
4. **Fully-Connected Layer**: A dense layer with one parameter: the output dimension.
5. **Flattening Layer**: Converts a series of convolutional filter maps to a column vector.
6. **Softmax Layer**: Converts final layer projections to normalized probabilities.

## Model Architecture

The model architecture will be specified in a text file. A sample architecture is provided below:


Conv 6 5 1 2

ReLU

Pool 2 2

Conv 12 5 1 0

ReLU

Pool 2 2

Conv 100 5 1 0

ReLU

FC 10

Softmax




## Training

- Backpropagation algorithm will be implemented for training the model.
- Weights will be updated using batch gradient descent, with gradients updated using a subset of the training set (ideally 32 samples) in each step.
- Two datasets will be used: MNIST and CIFAR-10, each containing 50k-60k samples.
- The evaluation set will be split into half, with 5k samples for validation and 5k samples for test purposes.
- Additionally, a toy dataset will be provided for testing the backpropagation algorithm implementation.

## Reporting Metrics

- Validation loss, accuracy, and macro-F1 score will be reported for each epoch (one pass over the full training set).
- The model will be trained for 5-10 epochs, with the learning rate starting from 0.001.
- The best model will be selected based on the macro-F1 score.

## Implementation Details

- No deep learning framework is allowed for implementation.
- No hardware acceleration is required (but allowed if desired).
- Code must be modularized to work for any architectures using the six mentioned layers.
- Each operation will be posed as matrix multiplication for efficiency.
