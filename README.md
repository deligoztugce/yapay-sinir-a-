# Neural Network Backpropagation Example

This repository contains an implementation of a simple neural network with one hidden layer and backpropagation. The network uses the sigmoid activation function and trains using gradient descent. The code demonstrates how to:

1. **Forward Propagation**: Calculate the outputs of each layer.
2. **Loss Calculation**: Compute the loss using Mean Squared Error (MSE).
3. **Backpropagation**: Perform weight updates based on the gradient of the loss.
4. **Weight Update**: Use the gradients to update the weights.

## Structure

- **Activation Functions**:
  - Sigmoid function for activation.
  - Sigmoid derivative for backpropagation.

- **Forward Propagation**:
  - Calculate the output of the network layers using weights and inputs.

- **Loss Function**:
  - Mean Squared Error (MSE) is used to compute the difference between predicted and target output.

- **Backpropagation**:
  - Gradient of the loss with respect to the weights is calculated and used to update the weights.

## Code Flow

1. **Initialization**:
   - Initialize the weights (`w1`, `w2`, etc.) and biases (`b1`, `b2`, etc.).
   - Define the input values (`i1`, `i2`) and the target output (`y`).

2. **Forward Propagation**:
   - The network consists of 2 input nodes, a hidden layer with 2 neurons, and an output layer.
   - Each layer performs a weighted sum followed by a sigmoid activation.
   - The final output is calculated.

3. **Loss Calculation**:
   - Calculate the loss using Mean Squared Error (MSE) between the predicted output and the target.

4. **Backpropagation**:
   - Compute the derivatives of the loss with respect to the output and hidden layer weights.
   - Apply the chain rule to propagate the error back through the network.
   - Update the weights using gradient descent.

5. **Training Loop**:
   - The network is trained for a specified number of epochs (100 in this case).
   - After each epoch, the weights are updated, and the loss is printed.

## Requirements

- Python 3.x
- NumPy library (`pip install numpy`)

## Running the Code

1. Clone the repository or download the Python script.
2. Install the necessary libraries using:
   ```bash
   pip install numpy
