# Deep-Learning
Deep Learning
## Background

The nonprofit foundation Alphabet Soup wants a tool that can help it select the applicants for funding with the best chance of success in their ventures. With your knowledge of machine learning and neural networks, you’ll use the features in the provided dataset to create a binary classifier that can predict whether applicants will be successful if funded by Alphabet Soup.

From Alphabet Soup’s business team, you have received a CSV containing more than 34,000 organizations that have received funding from Alphabet Soup over the years.

## Overview

## Results
### Data Processing
 * What variable(s) are the target(s) for your model?
   The target for the model is the indicator for a successful applicant: "IS_SUCCESSFUL" with the values 1 and 0
    The features included:
      * **APPLICATION_TYPE**—Alphabet Soup application type
     * **AFFILIATION**—Affiliated sector of industry
     * **CLASSIFICATION**—Government organization classification
     * **USE_CASE**—Use case for funding
     * **ORGANIZATION**—Organization type
     * **STATUS**—Active status
     * **INCOME_AMT**—Income classification
     * **SPECIAL_CONSIDERATIONS**—Special consideration for application
     * **ASK_AMT**—Funding amount requested
     * **IS_SUCCESSFUL**—Was the money used effectively?

 * What variable(s) should be removed from the input data because they are neither targets nor features?
     * Identification columns "EIN" and "NAME" were removed

## Results
### Compiling, Training, and Evaluating the Model
 * This model used four hidden layers with 150, 50, 10, and 3 nodes
 * Initially, the model did not yeild the desired 75% accuracy threshold. In the initial run of the model, there was one hidden layer, with 100 nodes, that yeilded a 49% accuracy. The activation of the model was "relu" in the hidden layer and "sigmoid" in the output. However, by adding additional hidden layers and incorporating additional optimizers softmax and tanh, accuracy was increased 72.78%. 
 Despite these efforts, the final accuracy did not meet the threshold. 