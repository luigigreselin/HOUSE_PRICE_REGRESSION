# HOUSE PRICE REGRESSION

Kaggle challenge to predict house prices in an unknown city given 81 features.

# Overview
I compared a number of different approaches from Random Forest (with a grid to refine the parameter estimation) to a fully connected neural network on Keras to predict the final house price.

# Data preprocessing
1. eliminated all those variables that had more than 50% empty values
2. filling the nan in the categorical variables with their mode, filling the numerical variables with their median (to avoid problems created by the outliers)
3. checking for multicollinearity between numerical variables and eliminated those with and Rsquared above 90%. 
4. With the chi square test I checked also the collinearity between categorical variables but the distributions of their levels were highly not uniform so I retained all of them.

# Results
With the random forest I obtained 84% of precision (not on the test dataset). I then created a 3-hidden layers NN on Keras and performed the analysis. On the test dataset (30% of my training data) I obtained a correlation of 88%.

# Data
Downloaded from [here](https://www.kaggle.com/c/house-prices-advanced-regression-techniques)
