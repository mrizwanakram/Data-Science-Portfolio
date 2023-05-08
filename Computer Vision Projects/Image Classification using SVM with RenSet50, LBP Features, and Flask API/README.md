# Image Classification using SVM with RenSet50, LBP Features, and Flask API

This is a project for image classification using Support Vector Machine (SVM) with RenSet50, Local Binary Pattern (LBP) Features, and Flask API. The project aims to classify images into multiple categories by using RenSet50, LBP Features, and SVM model.

## Project Requirements

- Python 3.6 or above
- Flask
- Scikit-Learn
- NumPy
- OpenCV

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
- `svm_model.py` - contains the script to create and train the SVM model using RenSet50 features, image width and height, and LBP features.
- `accuracy_metrics.py` - contains the script to auto-create accuracy metrics report for your SVM model.
- `app.py` - contains the Flask API code for image classification.
- `Dockerfile` - contains the instructions to build a Docker container for the Flask API.

## How to Use the API

1. Make a POST request to `http://localhost:5000/predict`.
2. Send an image file as a form-data with the key `file`.
3. The API will return the predicted category of the image.

## Why did we scale the data before passing it to SVM?

Scaling the data is important because SVM is sensitive to the scale of the features. If the scale of the features is not consistent, SVM will give more importance to the features with larger values. Scaling the features to the same scale can improve the performance of SVM and make sure that all features are given equal importance in the model.

## Conclusion

This project demonstrates how to use SVM with RenSet50, LBP Features, and Flask API for image classification. By following the setup instructions, you can run the project and use the API to predict the category of an image.
