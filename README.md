# Diabetes Prediction Using Machine Learning

## Overview

This repository contains a machine learning project aimed at predicting diabetes using various classification algorithms. The project includes data preprocessing, model training, and evaluation to determine the most effective model for predicting diabetes.

## Contents

- **Dataset**: Contains the dataset used for training and testing the models.
- **Models**: Includes the saved models after training.
- **Notebook**: Jupyter notebooks with detailed steps for data preprocessing, model training, and evaluation.
- **templates**: HTML templates for the web interface.
- **app.py**: Flask application to deploy the model as a web service.
- **requirements.txt**: List of dependencies required to run the project.

## Installation

1. Clone the repository:
    ```bash
    git clone https://github.com/Raja904/Diabetes_prediction_Machine_Learning.git
    cd Diabetes_prediction_Machine_Learning
    ```

2. Create and activate a virtual environment:
    ```bash
    python -m venv venv
    source venv/bin/activate  # On Windows use `venv\Scripts\activate`
    ```

3. Install the required dependencies:
    ```bash
    pip install -r requirements.txt
    ```

## Usage

1. To run the Flask application:
    ```bash
    python app.py
    ```

2. Open your web browser and go to:
    ```
    http://127.0.0.1:5000/
    ```

## Project Structure

- **.ebextensions/**: Configuration files for deploying the app on AWS Elastic Beanstalk.
- **.github/workflows/**: GitHub Actions workflows for CI/CD.
- **.vscode/**: VSCode configuration files.
- **Dataset/**: Folder containing the dataset.
- **Models/**: Folder containing the saved models.
- **Notebook/**: Jupyter notebooks for data preprocessing, model training, and evaluation.
- **templates/**: HTML templates for the web application.
- **app.py**: Main Flask application file.
- **requirements.txt**: Python dependencies.

## Model Performance

We trained four models and their performance metrics are as follows:

### Logistic Regression
- **Accuracy**: 0.70
- **Precision**: 0.87 (class 0), 0.38 (class 1)
- **Recall**: 0.73 (class 0), 0.61 (class 1)
- **F1-Score**: 0.79 (class 0), 0.47 (class 1)
- **Confusion Matrix**:
    ```
    [[132  50]
     [ 19  30]]
    ```

### Decision Tree
- **Accuracy**: 0.74
- **Precision**: 0.81 (class 0), 0.60 (class 1)
- **Recall**: 0.79 (class 0), 0.62 (class 1)
- **F1-Score**: 0.80 (class 0), 0.61 (class 1)
- **Confusion Matrix**:
    ```
    [[122  32]
     [ 29  48]]
    ```

### Naive Bayes
- **Accuracy**: 0.74
- **Precision**: 0.79 (class 0), 0.64 (class 1)
- **Recall**: 0.81 (class 0), 0.62 (class 1)
- **F1-Score**: 0.80 (class 0), 0.63 (class 1)
- **Confusion Matrix**:
    ```
    [[120  29]
     [ 31  51]]
    ```

### Support Vector Classifier (SVC)
- **Accuracy**: 0.75
- **Precision**: 0.83 (class 0), 0.59 (class 1)
- **Recall**: 0.79 (class 0), 0.65 (class 1)
- **F1-Score**: 0.81 (class 0), 0.62 (class 1)
- **Confusion Matrix**:
    ```
    [[126  33]
     [ 25  47]]
    ```

### Conclusion

The SVC model was chosen for deployment due to its highest accuracy (0.75) and balanced performance across other metrics, making it the most reliable model for predicting diabetes.

## Deployment

The model has been deployed and is accessible at:
[Predict Your Diabetes](https://predictyourdiabetes.azurewebsites.net/predictdata)

## Contributing

Contributions are welcome! Please create a pull request or open an issue to discuss what you would like to change.

## License

This project is licensed under the MIT License. See the LICENSE file for details.

## Acknowledgements

This project was inspired by the need to leverage machine learning for medical predictions and was developed using various online resources and tutorials.
