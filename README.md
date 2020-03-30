# CNN_Classification

## Project Overview

What we are trying to do here is train a CNN model which can provide an estimate of the dog's breed. If a human is detected, it will provide an estimate of the dog breed that is most resembling.

We are going to do it in 4 steps:

* Develop a model to detect humans
We use OpenCV's implementation of Haar feature-based cascade classifiers to detect human faces in images.

* Develop a model to detect dogs
In this section, we use a pre-trained ResNet-50 model to detect dogs in images. Our code downloads the ResNet-50 model, along with weights that have been trained on ImageNet.

* Develop a model to predict dog's breed
In this step, we will create a CNN that classifies dog breeds but without using any transfer learning.

* Improving the results using transfer learning
We will use the the pre-trained Xception model as a fixed feature extractor, where the last convolutional output is fed as input to our model.

## Required Libraries

* sklearn
* keras

## Acknowledgement

Thanks to Udacity for providing the platform

