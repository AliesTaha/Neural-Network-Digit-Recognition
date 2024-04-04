# Neural Network for Handwritten Digit Recognition

This project focuses on building and training a neural network model to recognize handwritten digits (0-9) using TensorFlow. It demonstrates the fundamental concepts of neural networks, including the ReLU activation function, softmax function for multiclass classification, and the implementation of these concepts using TensorFlow's Sequential API.

## Table of Contents

- [Project Overview](#project-overview)
- [Getting Started](#getting-started)
  - [Prerequisites](#prerequisites)
  - [Installation](#installation)
- [Dataset](#dataset)
- [Model Architecture](#model-architecture)
- [Training the Model](#training-the-model)
- [Evaluation and Prediction](#evaluation-and-prediction)
- [Results](#results)
- [Contributing](#contributing)
- [License](#license)
- [Acknowledgments](#acknowledgments)

## Project Overview

The project aims to classify images of handwritten digits (0-9) into their respective classes. It employs a neural network with two hidden layers using ReLU activation and an output layer designed for multiclass classification. The softmax function is utilized for converting model logits to probabilities during the loss calculation phase for improved numerical stability.

## Getting Started

These instructions will get you a copy of the project up and running on your local machine for development and testing purposes.

### Prerequisites

Before running this project, ensure you have the following software installed:

- Python 3.7 or later
- pip package manager

### Installation

1. Clone the repository to your local machine:

```bash
git clone https://github.com/your_username/neural-network-digit-recognition.git
```

2. Install the required Python packages:

```bash
pip install numpy matplotlib tensorflow
```

## Dataset
The dataset comprises 5000 training examples of handwritten digits from 0 to 9. Each digit is represented by a 20x20 pixel grayscale image, which is unrolled into a 400-dimensional vector for model training.
![image](https://github.com/AliesTaha/Neural-Network-Digit-Recognition/assets/103478551/0799d463-8139-4baa-b99c-2d4e2914a62f)

## Model Architecture
The neural network model consists of the following layers:

Input layer: 400 units (corresponding to the 20x20 pixel images).
First hidden layer: 25 units with ReLU activation.
Second hidden layer: 15 units with ReLU activation.
Output layer: 10 units with linear activation for multiclass classification.
Training the Model
The model is compiled with the Adam optimizer and SparseCategoricalCrossentropy loss function, which includes softmax logic for probability distribution. It is trained for 400 epochs to ensure adequate learning.
![image](https://github.com/AliesTaha/Neural-Network-Digit-Recognition/assets/103478551/5640dd37-0567-4f40-9a43-107447a4aaad)

## Evaluation and Prediction
Model performance is evaluated based on its accuracy in classifying the test images. Predictions are made by passing an image to the model and using the softmax function to convert the output logits to probabilities.

## Results
The model demonstrates high accuracy in recognizing handwritten digits. A sample of predictions versus actual labels can be seen in the project's Jupyter notebook.

## Contributing
Contributions to this project are welcome. Please fork the repository and submit a pull request with your changes.

