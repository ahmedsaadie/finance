# Imagerecongintion-Cat-vs-Non-Cat
using deep neural network for cat image recognition  
2 - Dataset
Problem Statement: dataset ("data.h5") containing:

- a training set of m_train images labelled as cat (1) or non-cat (0)
- a test set of m_test images labelled as cat and non-cat
- each image is of shape (num_px, num_px, 3) where 3 is for the 3 channels (RGB).
12,288  equals  64×64×3  which is the size of one reshaped image vector.

3 - Architecture of your model
a deep neural network to distinguish cat images from non-cat images.

Models are:

A 2-layer neural network
An L-layer deep neural network
Let's look at the two architectures.

3.1 - 2-layer neural network
3.2 - 5 -layer deep neural network

the Deep Learning methodology to build the model:
1. Initialize parameters / Define hyperparameters
2. Loop for num_iterations:
    a. Forward propagation
    b. Compute cost function
    c. Backward propagation
    d. Update parameters (using parameters, and grads from backprop) 
4. Use trained parameters to predict labels

- L-layer Neural Network
def initialize_parameters_deep(layers_dims): ... return parameters def L_model_forward(X, parameters): ... return AL, caches def compute_cost(AL, Y): ... return cost def L_model_backward(AL, Y, caches): ... return grads def update_parameters(parameters, grads, learning_rate): ... return parameters `
