# Individual-Medical-Costs-Prediction
This project is a Regression Analysis project aimed at predicting individual medical costs billed by health insurance. The goal is to build a regression model that can accurately predict the charges (medical costs) based on various features such as age, BMI, smoking status, region, etc.


# Individual Medical Costs Prediction

## Overview
This project aims to predict individual medical costs billed by health insurance using machine learning. The dataset contains information about individuals, such as age, gender, BMI, smoking status, region, and the number of children. The goal is to build a regression model that accurately predicts the `charges` (medical costs) based on these features.

This notebook contains the code for data preprocessing, exploratory data analysis (EDA), model training, evaluation, and deployment.



## Dataset Description
The dataset used in this project is publicly available and contains the following features:

### Features
- **age**: Age of the primary beneficiary (numeric).
- **sex**: Gender of the beneficiary (`male` or `female`).
- **bmi**: Body mass index (BMI) of the beneficiary (numeric).
- **children**: Number of children/dependents covered by health insurance (numeric).
- **smoker**: Smoking status of the beneficiary (`yes` or `no`).
- **region**: Residential area of the beneficiary (`northeast`, `southeast`, `southwest`, `northwest`).
- **charges**: Individual medical costs billed by health insurance (numeric, target variable).

### Dataset Source
The dataset is available on [GitHub](https://github.com/stedy/Machine-Learning-with-R-datasets/blob/master/insurance.csv).

---

## Installation
To run this project locally, follow these steps:

1. **Clone the repository**:
   ```bash
   git clone https://github.com/your-username/Individual-Medical-Costs-Prediction.git
   cd Individual-Medical-Costs-Prediction

   


# Usage
## Data Preprocessing:

The dataset is preprocessed to handle categorical variables using One-Hot Encoding (pd.get_dummies).

Numerical features are normalized using StandardScaler.

Exploratory Data Analysis (EDA):

Visualizations are created to understand the distribution of the target variable (charges) and the relationships between features.

## Model Training:

Multiple regression models are trained, including:

Linear Regression

Ridge Regression

Lasso Regression

Decision Tree Regressor

Random Forest Regressor

Gradient Boosting Regressor

XGBoost

LightGBM

CatBoost

Support Vector Regressor (SVR)

Multi-Layer Perceptron (MLP) Regressor

K-Nearest Neighbors (KNN) Regressor

Hyperparameter tuning is performed using Grid Search CV.

## Model Evaluation:

Models are evaluated using metrics such as:

Mean Absolute Error (MAE)

Mean Squared Error (MSE)

Root Mean Squared Error (RMSE)

R-squared (R²)

Saving the Best Model:

The best-performing model (Gradient Boosting) is saved using joblib.

Making Predictions:

The saved model can be loaded and used to make predictions on new data.


# Results
The best-performing model is Gradient Boosting, with the following evaluation metrics on the test set:

Mean Absolute Error (MAE): 2537.99

Mean Squared Error (MSE): 19652134.66

Root Mean Squared Error (RMSE): 4433.07

R-squared (R²): 0.8734

Feature Importance
The most important features for predicting medical costs are:

Smoking status (smoker_yes)

BMI

Age
