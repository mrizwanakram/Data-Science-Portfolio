
# Building an Image Classifier for Apple vs Banana with InceptionV3 and U-Net Architecture in TensorFlow Keras

## Introduction
This project aims to build an image classifier that can distinguish between images of apples and bananas using deep learning techniques. The model architecture consists of a U-Net like structure with InceptionV3 as the backbone. The code is written in TensorFlow Keras, a high-level neural network API that allows for easy and fast prototyping.

## Dataset
The dataset used in this project contains a collection of images of apples and bananas. The images are in JPEG format and have varying resolutions. The dataset is split into two directories, one for each class of fruit. I choose just Apple and bannana Images for traning.
#### Dataset Link: https://www.kaggle.com/datasets/sriramr/apples-bananas-oranges

## Model Architecture
The model architecture used in this project consists of a U-Net like structure with InceptionV3 as the backbone. The input images are preprocessed using various techniques such as normalization, resizing, and data augmentation. The output layer of the model is a binary classification layer that predicts whether an image is of an apple or a banana.

## Requirements
To run the code in this project, you will need the following packages:

- TensorFlow 2.x
- Keras
- Numpy
- Matplotlib
- OpenCV

## Usage
To train and test the model, run the `train.py` script. The script loads the dataset, preprocesses the images, builds the model, trains the model, and evaluates the model's performance. The model weights are saved to a file named `model.h5` in the current directory.

To predict the class of a new image, run the `predict.py` script. The script loads the model weights from the `model.h5` file, preprocesses the input image, and predicts the class of the image.

## Conclusion
In this project, we have successfully built an image classifier using deep learning techniques that can distinguish between images of apples and bananas. The U-Net like structure with InceptionV3 as the backbone proved to be an effective model architecture, achieving high accuracy on the test set. This project can be extended to other fruit types or to larger datasets with minimal modifications.
