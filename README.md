# Startup Success Prediction

## Project Overview
In this project, a machine learning model is created to predict the success of ventures funded by Alphabet Soup. The model is based on a dataset of more than 34,000 organizations that have received funding from Alphabet Soup over the years, containing various types of information about these organizations, including whether they became successful.

## Features
The dataset includes the following features:

- `EIN` - The organization's Employer Identification Number (EIN).
- `NAME` - The official name of the organization.
- Various features related to the type, presence, and operations of the organization.
- `IS_SUCCESSFUL` - Was the money used effectively.

The `IS_SUCCESSFUL` feature is the target for our binary classification.

## Methodology
The project follows these steps:

1. **Data Preprocessing**: The data is cleaned and preprocessed. Categorical variables are encoded using one-hot encoding, and the features are scaled using the StandardScaler from sklearn.

2. **Compile and Evaluate a Binary Classification Model Using a Neural Network**: A binary classification model is created using a deep neural network. The model's performance is assessed by its loss and accuracy.

3. **Optimize the Neural Network Model**: The model is optimized by adjusting the number of layers, the number of neurons in the layers, and the activation functions used in the neurons.

## Models
The base model includes two hidden layers with "relu" activation function and an output layer with "sigmoid" activation function, given it's a binary classification. The model is compiled using the adam optimizer and binary_crossentropy for the loss function.

Two additional models are tested to optimize the base model's performance:

- **Alternative Model 1**: This model includes three hidden layers instead of two. 
- **Alternative Model 2**: This model includes only one hidden layer.

## Requirements
This project uses Python and the following libraries and modules:

- pandas
- sklearn
- tensorflow

## Results
Model performance is compared based on the loss and accuracy metrics. The model with the best performance is selected.

## Future Work
Further optimization could include additional testing with more alternative models, adjusting additional parameters in the model, or collecting and adding more features to the dataset.
