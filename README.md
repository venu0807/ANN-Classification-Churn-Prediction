# ANN Classification - Churn Prediction

## Project Overview

This project focuses on predicting customer churn using an Artificial Neural Network (ANN). Customer churn prediction is essential for businesses to identify and retain at-risk customers by analyzing demographic and behavioral data. By leveraging deep learning, this project aims to improve the accuracy of churn prediction and provide a deployable solution via a web interface.

## Objective

- Develop a deep learning model using ANN to predict customer churn.
- Enhance skills in machine learning, model optimization, and deployment.
- Provide a user-friendly interface for businesses to predict customer churn using a Streamlit web application.

## Project Structure

ANN-Classification-Churn-Prediction/
├── Churn_Modelling.csv # Dataset used for training and evaluation
├── LICENSE # Project license
├── README.md # Project documentation
├── app.py # Streamlit app for deploying the churn prediction model
├── experiments.ipynb # Exploratory data analysis and initial model training
├── hyperparametertuning.ipynb # Hyperparameter tuning of the ANN model
├── label_encoder_gender.pkl # Pre-trained label encoder for gender
├── model.h5 # Trained ANN model saved in HDF5 format
├── onehot_encoder_geo.pkl # Pre-trained one-hot encoder for geography
├── predictions.ipynb # Model predictions on sample data
├── requirements.txt # Project dependencies
└── scaler.pickle # Pre-trained scaler for data preprocessing

## Model Details

The ANN model is structured as follows:

- **Input Layer:** Accepts numerical and encoded categorical features.
- **Hidden Layers:** Two fully connected dense layers with ReLU activation functions.
- **Output Layer:** A single neuron with sigmoid activation to perform binary classification (churn/no churn).

## Data Preprocessing

- **Label Encoding:** The Gender feature is encoded into numeric labels.
- **One-Hot Encoding:** The Geography feature is converted into multiple binary features.
- **Feature Scaling:** Numerical features such as Credit Score, Age, Balance, etc., are scaled using the StandardScaler to normalize the input data.

## How to Run the Project

### 1. Clone the Repository

```bash
git clone https://github.com/venu0807/ANN-Classification-Churn-Prediction.git
cd ANN-Classification-Churn-Prediction

### 2. Install Dependencies

Make sure Python (preferably 3.7 or above) is installed. Then install required packages:

pip install -r requirements.txt


3. Run the Streamlit Web Application

Launch the user interface to interact with the churn prediction model:

streamlit run app.py


This will open a local web app where you can input customer details and get churn predictions.

4. Explore Jupyter Notebooks

experiments.ipynb — For exploratory data analysis (EDA) and initial ANN model training.

hyperparametertuning.ipynb — For fine-tuning the ANN model hyperparameters.

predictions.ipynb — To test the trained model on new data samples.

Model Performance

The trained ANN model achieves an accuracy of approximately 86% on the test dataset, showing effective prediction capabilities for customer churn classification.


License

This project is licensed under the GPL-3.0 License. See the LICENSE
 file for more details.

For further information, contributions, or issues, please visit the GitHub repository.


---

If you want, I can also help you create a nicely formatted release note or instructions for contribution! Let me know.
