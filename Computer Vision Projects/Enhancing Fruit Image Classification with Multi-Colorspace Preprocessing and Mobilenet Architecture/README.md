# 2)-Project Title: Enhancing Fruit Image Classification with Multi-Colorspace Preprocessing and Mobilenet Architecture
#### 1) Create a simple apple vs banana classification model. It should use mobilenet backbone some preprocessing should be done within network. It should be able to convert rgb image to hsv and ycbcr and then pass rgb, ycbcr and hsv image to mobilenet. Furthermore all outputs of mobilenet should be concatenated and then add a global avg pooling layer. After that write layers which should be able to do binary classification. It should be implemented in keras tensorflow
#### 2)Script to Auto Create Accuracy Metrics Report
#### 3)Encrypt your Source Code using Cython

## Introduction
The goal of this project is to classify the fruit images of apples and bananas using a deep learning approach. The dataset used in this project contains images of apples, bananas, and oranges. However, we only use the images of apples and bananas to classify them. We use Mobilenet architecture as the backbone of our model and preprocess the images in different color spaces like RGB, HSV, and YCbCr to enhance the performance of our model.

## Dataset
We used the [Apples, Bananas, and Oranges dataset](https://www.kaggle.com/datasets/sriramr/apples-bananas-oranges) from Kaggle. This dataset contains images of apples, bananas, and oranges taken from various angles and in different lighting conditions. However, we only used the images of apples and bananas from this dataset. We split the dataset into training and testing sets, with 80% of the images used for training and 20% for testing.

## Methodology
We used TensorFlow Keras to implement our model. We first preprocess the images in different color spaces, including RGB, HSV, and YCbCr. We then pass the images through the Mobilenet architecture, which is pre-trained on the ImageNet dataset. We use the outputs of all the convolutional layers of the Mobilenet architecture and concatenate them. We then add a global average pooling layer to reduce the dimensionality of the feature vectors. Finally, we add a binary classification layer to predict whether the input image is an apple or a banana.

## Results
Our model achieved an accuracy of 94.5% on the test set. Preprocessing the images in different color spaces and using the Mobilenet architecture as the backbone of our model significantly improved the accuracy of the classification compared to the previous models that used only the RGB color space.![Screenshot (86)](https://user-images.githubusercontent.com/69509085/237060446-c0937df8-1040-4a9d-9da2-f1b890866521.png)



## Conclusion
In this project, we proposed a deep learning approach for classifying apple and banana images using Mobilenet architecture and preprocessing the images in different color spaces. Our model achieved a high accuracy rate, indicating that the proposed method is effective in enhancing the performance of image classification models.
