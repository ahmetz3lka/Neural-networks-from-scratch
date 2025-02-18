# Digit Recognition from Scratch Using NumPy

## Overview

This project implements a simple digit recognition system using only NumPy, without any deep learning frameworks like TensorFlow or PyTorch. The model is trained using a fully connected neural network from scratch to classify handwritten digits from the MNIST dataset.

## Features

- Implements a feedforward neural network with backpropagation
- Uses only NumPy for matrix operations and optimization
- Trains on the MNIST dataset
- Supports batch gradient descent
- Includes activation functions like ReLU and Softmax
- Uses cross-entropy loss for training

## Dataset

The project uses the [Digit Recognizer](https://www.kaggle.com/c/digit-recognizer/data), which consists of 42,000 training images of handwritten digits (0-9). The dataset is preprocessed by normalizing pixel values to the range [0, 1].

## Model Architecture

- **Input Layer**: 784 neurons (28x28 pixel images flattened)
- **Hidden Layer(s)**: Configurable number of neurons (for this I choose 10) with ReLU activation
- **Output Layer**: 10 neurons (for digits 0-9) with Softmax activation

## Installation & Setup

### Prerequisites

Ensure you have Python installed along with NumPy and Matplotlib for visualization.

### Installation

1. Clone this repository:
   ```bash
   git clone https://github.com/yourusername/digit-recognition-numpy.git
   cd digit-recognition-numpy
   ```
2. Install required dependencies:
   ```bash
   pip install numpy matplotlib
   ```
3. Run the notebook or script to train the model:
   ```bash
   python train.py
   ```

## Usage

- Load the dataset and preprocess the images
- Initialize and train the neural network
- Evaluate the model's performance on test data
- Visualize training loss and accuracy trends

## Results

After training, the model achieves around **89% accuracy** on the MNIST train set. The performance can be improved by tweaking hyperparameters such as learning rate, number of layers, and neurons per layer.

## Future Improvements

- Implement additional optimizers like Adam or RMSprop
- Add convolutional layers for better feature extraction
- Extend the model to recognize other handwritten characters

## Contributing

Feel free to fork this repository and contribute improvements!

## License

This project is licensed under the MIT License.
