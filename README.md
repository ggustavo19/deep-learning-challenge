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

  How many neurons, layers, and activation functions did you select for your neural network model, and why?
Were you able to achieve the target model performance?
What steps did you take in your attempts to increase model performance?
    *

  
## Summary

The Logistic Regression model used in this report came back with exceptional results that can accurately predict non defaults by 100% and defaults by 85%. The overall accuracy for the prediction model was 99% which makes it a highly accurate model to use in order to predict whether a borrower will default on their loan. 
