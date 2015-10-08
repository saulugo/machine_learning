#Machine Learning Foundations

#Abstract
My notes during the Machine Learning Foundation class at coursera.org

#Week 1 and 2

#Regression Models
The idea is that we have an observation value that is associated to a set of features, so we want to model how our observation value varies when we change the values of the features.

For example, we can model how a house value price varies (the observation) as a function of the house features (size, number of bathrooms and bedrooms, location, etc)

Others applications of regression are:
Classification: for example, we can use a regression model in other to classify emails as spam or not spam

##Some Terminology
In a regression model the X variable that is plotted in the X axis is called the predictor, or the covariate, or the feature or the independent variable
And Y is the observation or the dependent variable 

##Linear Regression Model
<img src="./img/ml_001.jpg">

Adding a higher order effects

For example using a quadratic function
<img src="./img/ml_002.jpg">

How to choose the model order/complexity

- Simulate predictions
	1) Remove some houses from the data we have
	2) Fit model on remaining
	3) Predict heldout houses
	
<img src="./img/ml_003.jpg">

Houses that we use to fit our model, we call it the training set
Houses that we use as a proxy for a prediction, those that we hold out, we call that the test set

<img src="./img/ml_004.jpg">

So, the training error is the RSS of the training dataset

So, we look at the parameters or features that minimize our training error

<img src="./img/ml_005.jpg">

The test error is the RSS for the observations that are in our test dataset
<img src="./img/ml_006.jpg">
As we increase the order of the model the training error tents to decrease and approximate to zero. However, at some point the predictions will be poor even if the training error is very small.

When we apply our model to the test dataset, and as we increase the order of the model, the test error will decrease improving the quality of the prediction. However at some point or at some model order, the test error will start to increase, deteriorating the quality of the prediction.

##Machine Learning - Regression Model Blocks Diagram
<img src="./img/ml_007.jpg">

