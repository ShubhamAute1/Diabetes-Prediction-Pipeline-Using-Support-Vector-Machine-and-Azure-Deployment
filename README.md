Overview

This repository contains a comprehensive machine learning pipeline to predict diabetes status using the PIMA Diabetes Dataset. The project includes data preprocessing, model training, evaluation, and deployment via an Azure-hosted API for real-time predictions.

Features

1. Data Preprocessing:
   Loads and cleans the PIMA Diabetes Dataset.
   Handles class imbalance using undersampling.
   Splits data into training and testing sets.

3. Model Training and Evaluation
   Trains a Support Vector Machine (SVM) classifier with a linear kernel.
   Evaluates the model using accuracy metrics on training and test data.

4. Predictive System
   Accepts user input (medical metrics) for real-time prediction.
   Outputs whether the individual is diabetic or not.

5. Model Deployment
   Saves the trained model as diabetes_model.pkl using pickle.
   Provides a script to interact with the deployed Azure API for predictions.

Project Structure
.
├── data
│   └── diabetes.csv        # Dataset
├── Diabetes_model.ipynb    # Model development and training notebook
├── prediction.ipynb        # Script for API interaction and testing
├── diabetes_model.pkl      # Saved model (after training)
├── README.md               # Project documentation



Installation

1. Clone the repository:
   git clone https://github.com/your-username/diabetes-prediction.git
   cd diabetes-prediction

2. Install dependencies:
   pip install -r requirements.txt
   Download the dataset and place it in the data directory.


Usage

1. Train the Model
   Open Diabetes_model.ipynb.
   Run all cells to:
   Preprocess the data.
   Train the SVM model.
   Evaluate its accuracy.
   Save the trained model.

3. Deploy the Model
   Use Azure ML Studio to deploy the trained model.
   Note down the scoring_uri for API interaction.

3. Make Predictions
   Open prediction.ipynb.
   Update the scoring_uri with the deployed endpoint URL.
   Run the script to make predictions.
