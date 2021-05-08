# Written Analysis of the Neural Metwork Machine Learning challenge Module 19

## Overview of Analysis
This project purpose is to use use deep-learning neural networks with the TensorFlow platform in Python, to analyze and classify the success of charitable donations.

We used the following methods for the analysis:

- preprocessing the data for the neural network model,
- compile, train and evaluate the model,
- optimize the model.


Data Source: 
![charity_data.csv] (https://github.com/archinarula/Neural_Network_Charity_Analysis/blob/main/charity_data.csv

## Deliverable: 
This challenge consists of three technical analysis deliverables and a written report.

- Deliverable 1: Preprocessing Data for a Neural Network Model
- Deliverable 2: Compile, Train, and Evaluate the Model
- Deliverable 3: Optimize the Model
- Deliverable 4: A Written Report on the Neural Network Model (README.md)



## Results

The results are displayed on Jupiter notebooks links 

![AlphabetSoupCharity.ipynb](https://github.com/archinarula/Neural_Network_Charity_Analysis/blob/main/AlphabetSoupCharity.ipynb) 

### Key findings and highlights of this analysis is:

Data Preprocessing
- What variable(s) are considered the target(s) for your model?
The column IS_SUCCESSFUL contains binary data to show if charity was successful or not. This variable is the target for our deep learning neural network.

- What variable(s) are considered to be the features for your model?
Columns APPLICATION_TYPE, AFFILIATION, CLASSIFICATION, USE_CASE, ORGANIZATION, STATUS, INCOME_AMT, SPECIAL_CONSIDERATIONS, ASK_AMT are the features for our model.

- What variable(s) are neither targets nor features, and should be removed from the input data?
Columns EIN and NAME are identification information and have been removed from the input data.

Compiling, Training, and Evaluating the Model
- How many neurons, layers, and activation functions did you select for your neural network model, and why?
This neuron network was made with two Hidden layers with 80 and 30 neurons.
ReLU activation function was used to spped up the training process.
Sigmoid was used on output layer which is a binary classification

- Were you able to achieve the target model performance?
No all 3 attempts gave the model accuracy of under 75%. This is not a satisfying performance to help predict the outcome of the charity donations.

- What steps did you take to try and increase model performance?
Applied bucketing to the feature ASK_AMT and organized the different values by intervals.
Attempt 1: Tried increasing number of neurons on one of the hidden layers, 
Attempt 2: Tried increasing number of hidden layers so school was informed. then used a model with three hidden layers.
Attempt 3: Tried a different activation function (tanh) 
but none of these steps helped improve the model's performance.


## Summary
The deep learning neural network model did not reach the target of 75% accuracy. Considering that this target level is pretty average we could say that the model is not outperforming.
Since we are in a binary classification scenario, we can use a supervised machine learning model such as the Random Forest Classifier to combine a multitude of decision trees to generate a classified output and evaluate its performance against our deep learning model.

 







 



