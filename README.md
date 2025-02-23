# House Price Prediction using Neural Networks

Welcome to the **House Price Prediction** project! This project demonstrates how to build and train a simple neural network to predict house prices based on the number of bedrooms. The model learns the relationship between the number of bedrooms and the corresponding price, making it a great introduction to linear regression with neural networks.

---

## Table of Contents
1. [Project Overview](#project-overview)
2. [How It Works](#how-it-works)
3. [Installation](#installation)
4. [Usage](#usage)
5. [Results](#results)
6. [Contributing](#contributing)
7. [License](#license)

---

## Project Overview

In this project, we create a neural network that predicts the price of a house based on a simple formula:
- A house has a base cost of **50k**.
- Each additional bedroom adds **50k** to the price.

For example:
- A 1-bedroom house costs **100k**.
- A 2-bedroom house costs **150k**.
- And so on.

The neural network learns this relationship and can predict the price of a house with any number of bedrooms.

---

## How It Works

1. **Data Generation**:
   - The training data consists of houses with 1 to 6 bedrooms and their corresponding prices in hundreds of thousands of dollars.
   - For example:
     - 1 bedroom → 1.0 (100k)
     - 2 bedrooms → 1.5 (150k)
     - 3 bedrooms → 2.0 (200k)

2. **Model Architecture**:
   - The model is a simple neural network with one dense layer.
   - It uses **Stochastic Gradient Descent (SGD)** as the optimizer and **Mean Squared Error (MSE)** as the loss function.

3. **Training**:
   - The model is trained for **500 epochs** on the generated data.

4. **Prediction**:
   - After training, the model can predict the price of a house with any number of bedrooms.
   - For example, it predicts the price of a 7-bedroom house as **4.0** (400k).

---

## Installation

To run this project, you'll need the following dependencies:

- Python 3.x
- TensorFlow
- NumPy

You can install the required libraries using `pip`:

```bash
pip install tensorflow numpy
