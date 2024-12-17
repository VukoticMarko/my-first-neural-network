# Simple Neural Network in Python

This is a minimal implementation of a single-layer neural network using Python and NumPy. The neural network can solve simple binary classification problems such as recognizing XOR-like patterns.

---

## Table of Contents

- [Introduction](#introduction)
- [Features](#features)
- [Installation](#installation)
- [Usage](#usage)
- [Example Output](#example-output)
- [How It Works](#how-it-works)
- [License](#license)

---

## Introduction

This neural network:
- Has **2 input neurons** and **1 output neuron**.
- Uses the **sigmoid activation function** to introduce non-linearity.
- Can train on simple binary combinations and predict outputs based on learned weights.

It is designed as a basic example to demonstrate how a neural network works internally, including forward propagation, error calculation, and weight updates using gradient descent.

---

## Features

- Single-layer neural network
- Customizable training iterations
- Training and validation error display every 10,000 iterations
- Lightweight: uses only NumPy
- Simple input/output handling for testing predictions

---

## Installation

To run this neural network, you need **Python 3** and **NumPy**.

1. Clone this repository or copy the code:
   ```bash
   git clone https://github.com/your-repo/simple-neural-network.git
   cd simple-neural-network

2. Install NumPy if it’s not already installed:
    pip install numpy

## Usage
Copy the neural network code into a Python file, e.g., neural_network.py.
Run the script:
python neural_network.py
Follow the prompts to input test values (binary inputs).

## Example Output
When you run the script, it will:

Print the randomly initialized weights.
Display training and validation error every 10,000 iterations.
Allow you to input two binary values for prediction.
Sample execution:

Random starting synaptic weights:
[[ 1.62434536]
 [-0.61175641]]

Iteration 0,
Training Error: 0.5
Validation Error: 0.5
-------------------------------------------------------
...
Iteration 10000,
Training Error: 0.5625520978699162
Validation Error: 0.24054312187155025
-------------------------------------------------------

Synaptic weights after training:
[[-4.36633509]
 [ 8.93927325]]

Input 1: 1
Input 2: 1
New input data (binary) = 11
New input data (decimal) = 3
Output data: 
[0.989778]

## How It Works
Initialization: Random weights are assigned.
Forward Propagation: Inputs are multiplied by weights, and the sigmoid function is applied.
Error Calculation: Error is calculated as the difference between actual and expected outputs.
Weight Adjustment: The weights are updated using gradient descent based on the error.
Training and Validation: The network trains iteratively and validates performance on a validation set.
Prediction: Once trained, the network can predict outputs for new inputs.

## License
This project is open-source and licensed under the MIT License. Feel free to use and modify it.
