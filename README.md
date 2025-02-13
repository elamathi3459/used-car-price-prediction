# CCC-Used-Car-Price-Prediction
## Spring 2022 CCC - IIT project
### Version
Python Version used: 3.7.13

### Packages
category_encoders scikit-learn matplotlib seaborn numpy sympy

## 1. Data_preprocessing

This file contains functions for data preprocessing and setting up the training and test sets. It comprises of functions for: category encoding, data preparation (including clearing null values, removing outliers, splitting into training and test sets etc.), and finally splitting the training and test sets into the predictor variables and response variable.

## 2. Model Training

### a. Extra Tree
This file simply contains a function for taking the training sets from the previous file and creating models using that data. It also contains a timer that tells you how much time it takes to train each model.

### b. Random Forest

This model is an ensemble learning method for classification, regression and other tasks. It works by constructing a multitude of decision trees at the training time. For Random Forest classification tasks, the output of the random forest is the class selected by most trees. This model also contains a timer that tells you how much time it takes to train each model.

### c. XGBoost

XGBoost is an optimized distributed gradient boosting library designed to be efficient, flexible, and portable. It implements machine learning algorithms under the Gradient Boosting framework. The main parameters of this trained model are obtained by hyperparameter grid search. The model also includes a timer that tells you how much time it takes to train each model.

## 3. Model Inference

### a. Extra Tree

This file simply contains a function for taking the training models produced by model training and performs inference and checks the accuracy and MAPE (mean absolute precentage error) of the prediction. It also contains a timer tat tells you the total time it takes to predict for both the voting the model and the regression models.

### b. Random Forest

This Regressor model builds decision trees on different samples and takes their majority votes for classification and average in case of regression. This model tells the time taken for voting the model and the regression models.

### c. XGBoost

This file contains a function for prediction. The prediction model is called in the file and the predicted result is checked by mape. It also calculates the total time required to vote for both predictive and regression models.
