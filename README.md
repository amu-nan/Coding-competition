# Directional Forecasting in Cryptocurrencies 
##### Predict whether crypto prices will surge or decline

#### This repository contains the solution for predicting cryptocurrency price movement using ensemble learning techniques involving Logistic Regression, Random Forest, and XGBoost. The project utilizes advanced feature engineering to enhance the model's ability to predict the direction of cryptocurrency prices.

## Project Overview

#### The goal of this project was to accurately predict whether the price of a cryptocurrency would move up or down based on historical data. Various machine learning models were implemented, and the final model is a blended ensemble that provided the best performance in terms of validation F1 score.

## Feature Engineering

#### To improve model performance, several feature engineering techniques were employed:

#### Lag Features: Created lag features for the 'close' price to capture temporal dependencies and trends.

#### Rolling Statistics: Generated rolling metrics such as mean, standard deviation, minimum, and maximum over different window sizes (5, 10, and 15) to capture short-term trends.

#### Time-Based Features: Extracted features such as hour, day of the week, and month to help the model understand temporal effects.

#### Class Imbalance Handling: Used SMOTE (Synthetic Minority Over-sampling Technique) to balance the dataset, ensuring better performance for minority classes.

## Final Model

#### The final solution is a blended ensemble of:
- Logistic Regression
- Random Forest Classifier
- XGBoost Classifier

#### These models were blended to leverage their strengths, leading to the best performance on the validation set. The ensemble model was used to generate predictions on the test set.

## Other Approaches Tried

#### CatBoost, Multi-layer Perceptron (MLP), and SARIMA models were also tested.

#### Stacking and Ensembling: Stacking various models including CatBoost, Random Forest, and XGBoost was explored, but blending proved to be more effective.

## Results

#### The blended model consisting of Logistic Regression, Random Forest, and XGBoost achieved the highest F1 score on the validation set, outperforming other combinations and individual models.

## Dependencies

#### The following Python libraries are required to run the project:

- pandas
- numpy
- matplotlib
- scikit-learn
- xgboost
- catboost
- imbalanced-learn
