# Experiment 08: Artificial Neural Networks using Keras

**Name:** R. Karthik  
**Roll No:** 25EU02904

## Pre-Lab Tasks

### 1. Basic Architecture of an Artificial Neural Network

An Artificial Neural Network (ANN) consists of an input layer, one or more hidden layers, and an output layer.

The input layer receives the input features. Hidden layers process the information using neurons. The output layer produces the final prediction.

Weights determine the strength of connections between neurons, while biases allow the model to shift the activation function and improve learning.

---

### 2. Activation Functions: ReLU and Sigmoid

ReLU (Rectified Linear Unit) is defined as:

ReLU(x) = max(0, x)

It is commonly used in hidden layers because it is computationally simple and helps neural networks learn nonlinear relationships.

Sigmoid converts a value into a range between 0 and 1:

Sigmoid(x) = 1 / (1 + e^-x)

It is commonly used in the output layer of binary classification models because its output can be interpreted as a probability.

---

### 3. Forward Propagation and Backpropagation

During forward propagation, input data passes through the network layer by layer. Each neuron calculates a weighted sum, adds a bias, and applies an activation function. The output is then compared with the actual target using a loss function.

Backpropagation calculates how much each network parameter contributed to the prediction error. The gradients of the loss with respect to the weights and biases are calculated and passed backward through the network.

The loss function measures the difference between predicted and actual values. The optimizer uses the calculated gradients to update the weights and biases so that the loss decreases during training.