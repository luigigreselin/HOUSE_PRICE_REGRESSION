# HOUSE_PRICE_REGRESSION
in this notebook I have been working on the open dataset from Kaggle on predicting house prices given a list of 81 variables. I compared a number of different approaches from Random Forest (with a grid to refine the parameter estimation) to a NN built on Keras.
I eliminated first all those variables that had more than 50% empty values, then I filled the nan in the categorical variables with the mode, and I filled the numerical variables with their
median (to avoid problems created by the outliers). I checked for multicollinearity between numerical variables and eliminated those with and Rsquared above 90%. With the chi 
square test I checked also the collinearity between categorical variables but the distributions of their levels were highly not uniform so I retained all of them.

Finally I performed a random forest to predict the price with a grid search to optimize the parameters. 
