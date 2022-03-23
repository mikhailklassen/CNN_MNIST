# Comparative implementations of convolutional neural nets against the MNIST dataset

This repository accompanies [this](https://medium.com/towards-data-science/tensorflow-vs-pytorch-by-example-66d37901c663) published in _Towards Data Science_.

An exercise in implementing the same CNN architecture in both PyTorch and Tensorflow. I have tried to keep the architecture, optimizer, learning rate, and scheduler the same across both implementation, but minor differences are inevitable. Both achieve similar accuracy of around 99% against the test set.

Each Notebook can be quickly launched in Google Colab using the links below. For GPU acceleration, remember to change your Notebook runtime to GPU.

## PyTorch Example
[![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/mikhailklassen/CNN_MNIST/blob/main/MNIST_PyTorch.ipynb)

## Tensorflow Example
[![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/mikhailklassen/CNN_MNIST/blob/main/MNIST_Tensorflow.ipynb)

# Data
In each example, we use the MNIST dataset. This data consists of 70,000 images of handwritten digits (0 to 9). Each image is a 28x28 pixel grid of grayscale values. As this is a common research dataset, both PyTorch and Tensorflow include their own helper functions for fetching this data. I have made use of these helper functions in each case.

# Acknowledgments
The PyTorch implementation is based off the example provided by the PyTorch development team, available in GitHub [here](https://github.com/pytorch/examples/blob/main/mnist/main.py). I made various modifications to this code in order to harmonize it with the Tensorflow example as well as to make it more amenable to running inside a Jupyter Notebook.

For the Tensorflow example, I made use of [Amy Jang](https://www.kaggle.com/amyjang)'s [tutorial on Kaggle](https://www.kaggle.com/code/amyjang/tensorflow-mnist-cnn-tutorial/notebook), which itself borrows from the Keras development team's [example](http://github.com/keras-team/keras/blob/master/examples/mnist_cnn.py) and the [tutorial](https://www.kaggle.com/code/yassineghouzam/introduction-to-cnn-keras-0-997-top-6/notebook) by [Yassine Ghouzam](https://www.kaggle.com/yassineghouzam). I again made various modifications to this code in order to harmonize it with the PyTorch example.
