# Neural_Network_Charity_Analysis

## Overview
This analysis entailed using the features in a provided dataset to help create a binary classifier that is capable of predicting whether applicants will be successful if they receive funding from AlphabetSoup. The dataset provided was a CSV containing more than 34,000 organizations that have received funding from AlphabetSoup over the years. To execute this analysis I utilized my knowledge of both machine learning and neural networks and completed the following required tasks:
* Deliverable 1: Preprocessing Data for a Neural Network Model
* Deliverable 2: Compile, Train, and Evaluate the Model
* Deliverable 3: Optimize the Model

## Results
*Data Preprocessing*
* The data in column __IS_SUCCESSFUL__ was the target variable for this model.
* There were two variables, the columns __EIN and NAME__, that were niether targets nor features leading me to remove them from the input data.
* The remaining 9 variables(columns) besides the target variable, IS_SUCCESSFUL, were the features for this model.

*Compiling, Training, and Evaluating the Model*
* For my neural network model I initially chose to use one activation function, ReLU, and 2 hidden layers with the first layer using 80 neurons while the second used 30 neurons. After not achieving the desired target model performance of 75% I decided to make 4 more varying attempts to accomplish the given goal. 
  * The __first attempt__ after the initail one I chose to add a third layer with 30 neurons and increased the first layers' neurons to 150 and the second layers' to 70. This attempt failed to achieve 75% accuracy so I moved along to a second attempt. 
  * The __second attempt__ was made by changing the activation function to __Tanh__ as well as lowering the amount of neurons in all three layers; the first layers' neurons was dropped to 100, the second layers' to 40, and the third layers' to 15. This attempt was also unsuccesful so I decided to once again lower the amount of neurons in the three hidden layers and change the activation function. 
  * The __third attempt__ involved changing the activation function back to __Relu__ as well as lowering the neurons within the three hidden layers. I lowered the first layers' neurons to 20, the second layers' to 8, and the third layers' to 3. My thinking behind lowering the amount of neurons was that throughout this module, all the models created had an accuracy of >80% by using only 8 neurons in the first layer and 3 neurons in the second layer. Continuing that line of thought I decided to make one last attempt.
  * The __fourth attempt__ included dropping back down to two hidden layers, changing the activation function to __Tanh__, and raising the amount of neurons within the hidden layers. In the first hidden layer I raised the neurons to 100 and in the second hidden layer I raised the neurons to 40. I was thinking that changing both the activation function and raising the neurons from original attempt may yield better results and accomplish the desired target model performance of 75%. I was unfortunately once again unsuccessful in achieving the goal.

## Summary 
Although attempting five different ways to create a model with 75% accuracy, all attempts were unsuccesful. All models achieved ~72.6% accuracy, failing to meet the target model performance. Being that this analysis is a binary classification, using the Random Forest Classifier which would combine multiple decision trees and generate a classified output, would be my recommendation to achieve the 75% target model performance that is desired. 
