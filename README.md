# deep-learning-challenge
Module 21 Challenge
Report - Deep Learning

The purpose of this analysis is to create and optimize a machine learning model that predicts whether an applicant for funding from Alphabet Soup will likely be successful. Using the dataset from Alphabet Soup, we aim to identify the features that most influence success and to build a binary classifier that can assist in selecting applicants with the highest potential for achieving their stated objectives. This predictive model will help streamline decision-making, ensuring that funding is allocated to applicants with the best chances of a successful outcome.

The dataset included the following columns:
EIN and NAME—Identification columns
APPLICATION_TYPE—Alphabet Soup application type
AFFILIATION—Affiliated sector of industry
CLASSIFICATION—Government organization classification
USE_CASE—Use case for funding
ORGANIZATION—Organization type
STATUS—Active status
INCOME_AMT—Income classification
SPECIAL_CONSIDERATIONS—Special considerations for application
ASK_AMT—Funding amount requested
IS_SUCCESSFUL—Was the money used effective

Results

Initial model structure
Layers:

The initial structure used two hidden layers.
First hidden layer: 80 neurons, ReLU activation function.
Second hidden layer: 30 neurons, ReLU activation function.
Output Layer: A single neuron with a sigmoid activation function

Activation Functions: ReLU for the hidden layers, Sigmoid for the output layer.

Performance
Initial Model: After training the model on 100 epochs, the accuracy achieved was approximately 72.75%. This was below the target performance accuracy of 75%.

Optimization Steps
In the additional optimization steps, I added third hidden layer, dropped only the EIN column, and then added more neurons to a hidden layer.

- Adding a third hidden layer resulted in an accuracy score of 72.98% which was still below the 75% threshold.
- Dropping only the EIN column and not the Name column resulted in a score of 72%.
- Adding additional neurons to our second hidden layer resulted in a score of 72.88%

Summary
I achieved the best result when I added a hidden layer to the model, though the improvement was not very significant compared with the other changes. For my optimization trials, I changed one aspect at a time in order to ensure that I could pinpoint the actions that caused changes in the accuracy score. I believe that combining the changes, for example adding both more additional hidden layers and more neurons, could possibly increase the accuracy score.
