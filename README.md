# Overview
## Purpose
Utilizes neural networks from the PyTorch library to classify 60,000 images of the CIFAR-10 dataset.

## Background
The CIFAR-10 dataset consists of 60000 32x32 colour images in 10 classes, with 6000 images per class. There are 50000 training images and 10000 test images.

The dataset is divided into five training batches and one test batch, each with 10000 images. The test batch contains exactly 1000 randomly-selected images from each class. The training batches contain the remaining images in random order, but some training batches may contain more images from one class than another. Between them, the training batches contain exactly 5000 images from each class.

Here are the classes in the dataset, as well as 10 random images from each:
airplane										
automobile										
bird										
cat										
deer										
dog										
frog										
horse										
ship										
truck										

The classes are completely mutually exclusive. There is no overlap between automobiles and trucks. "Automobile" includes sedans, SUVs, things of that sort. "Truck" includes only big trucks. Neither includes pickup trucks.

Ref: https://www.cs.toronto.edu/~kriz/cifar.html

## Packages
matplotlib.pyplot, seaborn, torch, torchvision

## Results
Reached 65% accuracy within 10 epochs for last layer.
![Results](https://github.com/jung2shinho/ML_ImageClassification/blob/main/accuracies.png)
## Neural Network Architecture
![Neural Network](https://github.com/jung2shinho/ML_ImageClassification/blob/main/nn_diagram.svg)

## How the Model Works
Creates four seperate models that uses convolution and max pooling of varying combination and number of layers. Rectified linear unit is utilized as the activation function for all models. 

## User Interface 
Jupyter Notebook. App not implemented yet.

## Code Structure
-.venv<br>
-data
--cifar-10-batches-py
--cifar-10-python.tar.gz
-accuracies.png
-nn_diagram.svg
-README.md<br>
-requirements.txt
