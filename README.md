# Neural Network Charity Analysis
This analysis aims to explain the neural network model we created to determine whether certain projects will or will not be successful. 

## Results

IS_SUCCESSFUL was the target for the model since we wanted it to determine the likelihood of successful projects. The two features I wanted to consider for the model included STATUS and IS_SUCCESSFUL because we wanted to determine whther applicatns that were actually funded by Alphabet Soup would be successful. 

Features that could've been removed include EIN, NAME, APPLICATION_TYPE, AFFILIATON, and CLASSIFICATION. Additionally, we could consider removing SPECIAL_CONSIDERATIONS, INCOME_AMT, ASK_AMT, USE_CASE and ORGANIZATION, though those features could be useful in detecting other trends that contribute to whether a project is sucessful or not. 

## Attempts to optimize the model

When attempting to optimize the model to increase predictive accuracy to mroe than 75%, I made the following adjustments: 
- Removed noisy variables so that the focus was on IS_SUCCESSFUL 
- Added additional neurons and a third hidden layer
- Changed the activation function in the hidden layers from ReLU to Tahn, but I kept the output function as sigmoid since our goal is to predict the probability of a project succeeding, meaning it could fall into one of two categories. 

## Recommendation 

For a request like this that asks us to determine whether or not a project has a chance of succeeding, we should consider using a logistic regression model since we're facing a binary classification problem and the dependent variable is dichotomous.  
