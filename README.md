# CIS_585_Project
Find my code here for the final project where I created SVM model and implemented it for Breast Cancer Classification

A little bit about the algorithm

This code defines a function `sgd` that implements Stochastic Gradient Descent algorithm for linear regression. The function takes two input arguments, `features` and `outputs`, which are the features and corresponding outputs of a dataset respectively. The function returns a weight vector that best fits the data according to the linear regression model.

The algorithm works by initializing the weight vector with zeros, shuffling the data to prevent any repeating update cycles, and then looping over the data points to update the weights using the gradient of the cost function. The cost function used here is the mean squared error between the predicted and actual outputs.

The algorithm also checks for convergence after every 2^n epochs, where n is incremented by 1 at every convergence check. Convergence is checked by computing the change in cost between consecutive epochs, and stopping the algorithm if the change in cost is less than a threshold value. If the algorithm does not converge, it terminates after a maximum number of epochs, which is set to 5000 in this case.

The learning rate, which controls the step size taken during weight updates, is set to a fixed value of 0.000001 in this code.
