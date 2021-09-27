# xgboost-car-price-prediction

The goal of this project is to solve a multiclass classifcation problem for a kaggle compe-
tition (https://www.kaggle.com/c/ugrin2020-vehiculo-usado-multiclase/overview). 

# data
The dataset contains data about cars sold, and the attribute to predict
is the car price that has been classified into  five categories (1- represents the
cheapest, 2- represents those cheaper then average, 3- represents those who are
in average price, 4- represents those who are more expensive than the average,
and 5- which represents the most expensive cars). 
The training set contains around 6000 samples and 13 attributes, both categorical and numerical data.
The class distribution is unbalanced. 

# solution
The best results were obtained by the XGBoost Classifier (Extreme Gradient
Boosting Algorithm) using following methods:
* imputing missing values
* label encoding
* feature selection (correlation matrix, chi-square test, mutual info gain)
* oversampling minority class using BorderlineSMOTE algorithm
A score of 0.80845 is achieved on the test set (0.8401 on
the training set). 

# file info
The documentation (pdf file) will describe the different methods of the solution, including the data
preprocessing applied in the best result and mention other strategies (removing chars from attributes, imputing missing values and encoding techniques, 
oversampling data) that were
tried out during the competition. 

KaggleSubmissions.pdf contains the table with information about every submission made to
kaggle during the competion.
