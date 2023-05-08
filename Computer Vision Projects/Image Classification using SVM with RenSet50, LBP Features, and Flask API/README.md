# Image Classification using SVM with RenSet50, LBP Features, and Flask API

This is a project for image classification using Support Vector Machine (SVM) with RenSet50, Local Binary Pattern (LBP) Features, and Flask API. The project aims to classify images into multiple categories by using RenSet50, LBP Features, and SVM model.Following are the Tasks that i do in this Project.

### 1) Create a simple SVM model which takes renset50 features, image width and height, image's lbp features. You should first create a csv of all features and then train svm. Before training svm. You should scale your data too.

### 2) Explain in the code why did we scale the data before passing it to svm

### 3) Script to Auto Create Accuracy Metrics Report

### 4) Create Model's Flask API

### 5) Docker file of API

## DataSet 
Dataset link: https://www.kaggle.com/datasets/hasibalmuzdadid/shoe-vs-sandal-vs-boot-dataset-15k-images

#### Context
This Shoe vs Sandal vs Boot Image Dataset contains 15,000 images of shoes, sandals and boots. 5000 images for each category. The images have a resolution of 136x102 pixels in RGB color model.

#### Content
There are three classes here.

Shoe
Sandal
Boot
#### Inspiration
This dataset is ideal for performing multiclass classification with deep neural networks like CNNs.
You can use Tensorflow, Keras, Sklearn, PyTorch or other deep/machine learning libraries to build a model from scratch or as an alternative, you can fetch pretrained models as well as fine-tune them.

#### Acknowledgement
This dataset is a modified version of a large image dataset provided by M.Stephenson.

## Project Requirements

- Python 3.6 or above
- tensorflow
- Flask
- Scikit-Learn
- NumPy
- OpenCV
- traceback
- base64
- time
- joblib
- pickle
- io
- argmax

## Project Setup

1. Clone the repository.
2. Install the required libraries using `pip install -r requirements.txt`.
3. Prepare your dataset and create a CSV file containing RenSet50 features, image width and height, and LBP features.
4. Run the script to create the SVM model that takes RenSet50 features, image width and height, and LBP features, scales the data, and trains the SVM model using the CSV file. The script also includes a description of why we scaled the data before passing it to SVM.
5. Run the script to auto-create accuracy metrics report for your SVM model.
6. Run the Flask API by executing the `app.py` file.
7. Access the API through `http://localhost:5000/predict` to predict an image's category.

## Files Description

- `README.md` - contains the project description and setup instructions.
- `requirements.txt` - contains all the required libraries for the project.
- `1&3-SVM Model Training from CSV and Auto Report Generating.ipynb` - contains the script to create and train the SVM model using RenSet50 features, image width and height, and LBP features.
- 2 why nead scaling: contains anser of question why we need scalling before SVM
- `3accuracy_metrics.txt` - contains the accuracy metrics report for my SVM model.
- `4-Flask API Server side and clint Side` - contains the Flask API code for image classification.
- `Dockerfile` - contains the instructions to build a Docker container for the Flask API.

## How to Use the API

1. Make a POST request to `http://localhost:5000/predict`.
2. Send an image file as a form-data with the key `file`.
3. The API will return the predicted category of the image.

## Why did we scale the data before passing it to SVM?

Scaling the data is important because SVM is sensitive to the scale of the features. If the scale of the features is not consistent, SVM will give more importance to the features with larger values. Scaling the features to the same scale can improve the performance of SVM and make sure that all features are given equal importance in the model.

## Conclusion

This project demonstrates how to use SVM with RenSet50, LBP Features, and Flask API for image classification. By following the setup instructions, you can run the project and use the API to predict the category of an image.
