Custom Linear Regression class has been created, which can be used to work with only 1 feature and 1 predictor. This
class
is a basic representation of how linear regressions work at its core, it uses gradient descent optimization for
parameter estimation. In a “magic method” __init__ I configure the learning rate, number of epochs, and convergence
threshold as well as randomly initialize the weights. In the fit method, weights updated based on the calculated
gradients using update weights and predict methods and then the cost function(mean squared error) is calculated to get
the error. This runs in a loop until the number of epochs is reached or when the difference between the old cost
function
and the new one is smaller than the threshold.

For the dataset, Scikit-learn’s diabetes dataset has been used.
Then I used dimensionality reduction technique(PCA in this case) to get only one feature to work with the linear
regression class.
Finally, I compared the performance of the custom linear regression class with the results of Scikit-learn’s regression.