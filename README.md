# deep-learning-challenge
Repository for UPenn Data Science Bootcamp Module 21 Challenge

## Overview of the Analysis
The purpose of this analysis was to develop a tool for the nonprofict foundation Alphabet Soup that would aid in selecting applicants for funding with the best chances of success in their ventures.  To do this, we used a dataset containing historical funding data from the nonprofit, machine learning, and a neural network to create a binary classifier that would predict whether ventures would be successful or not if being funded by Alphabet Soup with 75% accuracy. To preprocess the data, we completed the following steps:

* Drop the EIN and NAME columns
* Take counts of the data in the other features and bin small counts into an "other" category
* Use one-hot encoding to turn categorical data in the features into numeric data
* Split the data into target variables and features and use the standard scaler to scale the data
* Compile, train, and evaluate the model

## Results
* Model 1
    * Utilized 2 hidden layers
    * Used relu activation models for both hidden layers
    * Resulted in 72.9% accuracy

* Model 2
    * Utilized 2 hidden layers
    * Used tanh activation models for both hidden layers
    * Resulted in 72.7% accuracy

* Model 3
    * Utilized 3 hidden layers
    * Used relu activation models for each hidden layer
    * Resulted in 72.8% accuracy
    
## Summary
After 3 attempts at optimation, we did not achieve our goal of 75% accuracy.  When hidden layers and number of nodes were kept the same, the use of tanh as the activation function produced a slightly less accurate result than the relu activation function.  With the addition of an extra hidden layer and using the original relu activation function, we were able to slightly improve our result, but the original model produced the highest accuracy.  Because we were creating a binary classifier, I would attempt to use logistic regression and create a supervised learning model to try to improve the accuracy.