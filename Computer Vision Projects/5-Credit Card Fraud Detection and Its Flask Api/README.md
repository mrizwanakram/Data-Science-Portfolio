
# Credit Card Fraud Detection And Flask API

This project focuses on building a Credit Card Fraud Detection system using machine learning techniques. The dataset used for training and evaluation can be found at [Kaggle](https://www.kaggle.com/datasets/mlg-ulb/creditcardfraud).

## Project Structure

- `Flask_Api_Clint_Side.ipynb`: This Jupyter Notebook contains the client-side implementation of the Flask API. It demonstrates how to send requests to the API and receive responses.

- `Flask_Api_Server_side.ipynb`: This Jupyter Notebook contains the server-side implementation of the Flask API. It shows how to set up the API endpoints and handle incoming requests.

- `Task_7_Solution.ipynb`: This Jupyter Notebook presents one solution for the credit card fraud detection task. It includes data preprocessing, model training, and evaluation.

- `Task_7_Solution_2.ipynb`: This Jupyter Notebook provides an alternative solution for the credit card fraud detection task. It may contain different approaches, algorithms, or variations of the model.

- `credit_card_fraud_detection_model.joblib`: This file contains the trained model weights saved using the joblib library. It can be loaded and used for making predictions in the Flask API.

- `rf_model.pkl`: This file contains the trained model weights saved using the pickle library. It can also be loaded and used for making predictions in the Flask API.

## Getting Started

To set up and run the project, follow these steps:

1. Clone the repository:
   ```
   git clone https://github.com/Data-Science-Portfolio/Computer Vision Projects/5-Credit Card Fraud Detection and Its Flask Api.git
   cd credit-card-fraud-detection
   ```

2. Install the required dependencies. It is recommended to use a virtual environment:
   ```
   python -m venv venv
   source venv/bin/activate  # for Unix/Linux
   venv\Scripts\activate  # for Windows
   pip install -r requirements.txt
   ```

3. Download the dataset:
   - Download the dataset from the Kaggle link provided.
   - Place the dataset file (`creditcard.csv`) in the project's root directory.

4. Run the Flask API server:
   ```
   python Flask_Api_Server_side.ipynb
   ```

5. Use the client-side notebook (`Flask_Api_Clint_Side.ipynb`) to interact with the API. It demonstrates how to send requests and receive responses.

## Model Deployment

The trained model can be deployed using the Flask API. The server-side notebook (`Flask_Api_Server_side.ipynb`) provides the necessary code for setting up the API endpoints and loading the model weights.

## Contributing

Contributions are welcome! If you find any issues or have suggestions for improvements, please open an issue or submit a pull request.

## License

This project is licensed under the [MIT License](LICENSE).

Feel free to update and customize this README file based on your specific project requirements. Provide clear instructions, necessary dependencies, and any other relevant information to help users understand and utilize the Credit Card Fraud Detection Flask API effectively.
