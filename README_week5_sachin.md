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
For building a neural network, I have used a keras and gridsearchCV.
GridsearchCV was used to find the number of layers, neurons and suitable activation function.
Finally with keras I developed a neural network having 1 hidden layer with 30 neurons and a output layer with 1 output neuron.
Used relu activation function for hidden layers and linear activation function for the output layer, for optimizer i have used momentum gradient descent and mean absolute error for calculating the losses .
Finally I have used the neural network for predicting the unknown diameters of the asteroids.

