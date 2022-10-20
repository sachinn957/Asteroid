# Asteroid
Problem Statement
The diameter of an asteroid is one the most important physical parameter of an asteroid, 
it is used to detect if an asteroid is potentially hazardous or not if it is found to be a Near Earth Object. 
We aim to train a ML/DL model on JPL asteroid database to predict asteroid diameter.

# APPROACH
I have done some data visualization using matplotlib and seaborn and some data analysis using numpy.
For data cleaning
based on the correlation of different features with diameter and its variation , and which have more 90% missing values
I have dropped some features namely,
['H','albedo','name','rot_per','spec_B','BV','spec_T','UB','G','extent','GM','IR','neo','pha']
and used one hot encodding for condition code and class.
then split the data into train and test data.
I have applied various models including random forests , xgboost, neural network, linear regression
and based on the score , based on the score i have selected the basic NN model.

