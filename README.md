# deep-learning-challenge
GT DA Bootcamp Module 21 Challenge

## Overview
The purpose of this analysis is to create a binary classifier that can predict whether applicants would be successful if received funding from Alphabet Soup.

## Results
### Data Preprocessing
* What variable(s) are the target(s) for your model? What variable(s) are the features for your model? What variable(s) should be removed from the input data because they are neither targets nor features?
Removed variables: "EIN" and "NAME" 
Feature variables: The remaining columns.
The target variable for the model is "IS_SUCCESSFUL".

### Compiling, Training, and Evaluating the Model

* How many neurons, layers, and activation functions did you select for your neural network model, and why?
Initial model: Two layers. First layer had 80 neurons, and second layer had 30 neurons. I used the 'relu' activations for these two hidden layers and 'sigmoid' activation function for the output layer since this is a classification model.
Optimized model: Three layers. 50 neurons for the first layer, 30 neurons for the second layer, and 20 neurons for the third layer. Used 'relu" activation functions for the three hidden layers and 'sigmoid' activation function for the output layer since this is a classification model.

* Were you able to achieve the target model performance?
The optimized model achieved 75% accuracy (76.8%).

* What steps did you take in your attempts to increase model performance?
1) Dropped fewer columns (kept 'NAME')
2) Created more bins for rare occurrences in 'APPLICATION_TYPE' and 'CLASSIFICATION'.
3) Added more hidden layers


## Summary
The optimized model can show moderate success (with 76.8% accuracy) in predicting the whether an applicant would be successful if funded.
