# Diamond price competition
## Who will best predict the price of diamonds?

<img src=https://petalofucsia.blogia.com/upload/externo-1c5be1af60549d1a93eb01d0bb546771.jpg alt="drawing" width="200"/>

This is a kaggle competition, where a training set and a validation set are given to the players. The goal is to make the best model to predict the price of diamonds.

## 1. Data overview
With the seaborn library, regression, correlation and boxplots have been plotted. We found that cut, color and clarity features have no statistical differences in price. However, carat and dimensions of the diamond are very correlated to the price.

## 2. First models with sklearn library
This is a regression problem, so regression models have been used. 

After trying different options with the raw data, we could see that the models Random Forest Regressor, Kneigbors Regressor and Gradient Boost Regressor were converging towards the same solution.

## 3. Modeling with H2O
H2O is a python library with an AutoML function that trains the data with different models. This library has been used to make a better prediction without needing specifying any model parameter. In this step, data has been normalized, categorized and outliers have been removed, obtaining a RMSE in the training set of 521.
