# Neural Network Report

## Overview of the Analysis
The purpose of the analysis was create a binary classifier that can predict whether applicants will be successful if funded by Alphabet Soup. The meta data was on the following: APPLICATION_TYPE, AFFILIATION, CLASSIFICATION, USE_CASE, ORGANIZATION, STATUS, INCOME_AMT, SPECIAL_CONSIDERATIONS, and ASK_AMT. 

## Results

* Data Preprocessing
    * Target Variable:
      * `IS_SUCCESSFUL` Indicates whether the venture was successful or not
    * Feature Variables:
      * `EIN` and `NAME`—Identification columns
      * `APPLICATION_TYPE`—Alphabet Soup application type
      * `AFFILIATION`—Affiliated sector of industry
      * `CLASSIFICATION`—Government organization classification
      * `USE_CASE`—Use case for funding
      * `ORGANIZATION`—Organization type
      * `STATUS`—Active status
      * `INCOME_AMT`—Income classification
      * `SPECIAL_CONSIDERATIONS`—Special considerations for application
      * `ASK_AMT`—Funding amount requested
      * `IS_SUCCESSFUL`—Was the money used effectively
    * Removed Variables:
      * `EIN` and `NAME` were removed because they were Identification columns which did not aid with predictive information.
        
* Compiling, Training, and Evaluating the Model
    * Neurons, Layers, and Activation Functions:
      * First Hidden Layer: 8 neurons, `ReLU` activation function
      * Second Hidden Layer: 4 neurons, `ReLU` activation function
      * Third Hidden Layer: 2 neurons, `ReLU` activation function
      * Output Layer: 1 neuron, `Sigmoid` activation function
      * ![image](https://github.com/ggustavo19/deep-learning-challenge/assets/152371383/d48705e5-fbc5-4ea8-8187-851da843ca78)

      * Why: The edits on the 4th attempt were made to capture the patterns in the data. Originally the first attemp was 2 hidden layers with 80 and 30 units. The 2nd attempt had 12 units for both layers and changed to 150 EPOCHS instead of 100. The 3rd attempt had 12 units with hidden layers changed to activation function `Tanh` and 80 EPOCHS. All attemps were experimental to attempt a higher accuracy of over 75%. I was unfortunately not able to achieve the target performance with these methods. 

## Summary

The deep learning model developed with the highest accuracy out of the 3 optimization attempts was 73.05% which did not meet the 75% target. Additional layers were added, neurons were added and subtracted, different activation functions were made, and EPOCHS were also altered to train the model. I would recommend to attempt using Random forest model or create a Sequential model with hyperparameter options with running `kerastuner` to search for the best hyperparameters.

