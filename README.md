# Machine-Learning---House Price Prediction
# Project Overview:
The goal of this project is to predict house prices based on various features using a machine learning model. The dataset contains information about houses, including their attributes and prices, which will be used to train a predictive model.

# Dataset:
The dataset used for this project includes various features related to houses. Some key features are:

OverallQual: Overall material and finish quality

GrLivArea: Above grade (ground) living area square feet

GarageCars: Size of garage in car capacity

GarageArea: Size of garage in square feet

TotalBsmtSF: Total square feet of basement area

1stFlrSF: First-floor square feet

FullBath: Full bathrooms above grade

TotRmsAbvGrd: Total rooms above grade (does not include bathrooms)

YearBuilt: Original construction date

YearRemodAdd: Remodel date (same as construction date if no remodeling or additions)

# Data Preprocessing:

### Handling Missing Values:
a. Categorical features with missing values are filled with their mode.
b. Numerical features with missing values are filled with their mean.
### Encoding Categorical Features:
a. Categorical features are converted into numerical format using label encoding.
### Feature Scaling:
a. Numerical features are scaled using Min-Max scaling to normalize the data.

# Feature Selection:
The features selected for modeling are based on their correlation with the target variable SalePrice. The selected features include:

OverallQual
GrLivArea
GarageCars
GarageArea
TotalBsmtSF
1stFlrSF
FullBath
TotRmsAbvGrd
YearBuilt
YearRemodAdd

# Model Training:
Several machine learning models are trained and evaluated to find the best performing model:
>Linear Regression
>Decision Tree Regressor
>Random Forest Regressor
>Gradient Boosting Regressor

The dataset is split into training and testing sets with a ratio of 80:20. Each model is trained on the training set and evaluated on the testing set.

# Model Evaluation:
The performance of each model is evaluated using the Mean Absolute Error (MAE) and Root Mean Squared Error (RMSE) metrics. The model with the lowest MAE and RMSE is considered the best model for predicting house prices.

# Results:
Linear Regression:
MAE:2395020201.37
RMSE:0.33
Decision Tree Regressor:
MAE: 2042050380.27
RMSE: 0.43
Random Forest Regressor:
MAE: 1109397836.50
RMSE:0.43

# Conclusion:
The Random Forest Regressor was selected as the final model for predicting house prices. This model demonstrated the lowest error rates on the test dataset and provided the most accurate predictions.
