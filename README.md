#  Digit Classification using a Neural Network (NumPy Only)

This project implements a simple 2-layer neural network from scratch using only NumPy to classify handwritten digits from the MNIST dataset (Kaggle’s Digit Recognizer). The model learns to identify digits (0 to 9) by adjusting weights and biases using the backpropagation algorithm and gradient descent.

The network architecture consists of:
- Input layer: 784 neurons (one for each pixel in a 28x28 image)
- Hidden layer: 10 neurons with ReLU activation
- Output layer: 10 neurons with Softmax activation (one for each digit)

The data is preprocessed by normalizing pixel values (0–255) to the range [0, 1], and labels are one-hot encoded to work with softmax loss. We shuffle the dataset to prevent any bias and split it into training (41,000 examples) and development (1,000 examples) sets.

Backpropagation is used to compute the gradients of the loss with respect to each parameter (weights and biases), determining how much each should be adjusted. The model is trained over multiple iterations using gradient descent.

After training, the model achieves an accuracy of 87% on the training data.

This project is a pure implementation of the core logic behind neural networks and is designed for educational purposes — helping you understand forward propagation, backpropagation, softmax classification, and one-hot encoding without any machine learning libraries.
