# Model Report
1. The purpose of this report is to describe the neural network models that were created to predict the probability of success for applicants funded by Alphabet Soup and how these models performed.
2.  Results:
 * Target variable: IS_SUCCESSFUL - a binary int value that describes whether or not the applicant was successful
 * Features:
     * APPLICATION_TYPE_* - a binary int value that describe whether an applicant is part of a particular application category
     * AFFILIATION - Affiliated sector of industry
     * CLASSIFICATION_* - a binary int value that describe whether an applicant is part of a particular government classification category
     * USE_CASE - Use case for funding
     * ORGANIZATION - Organization type
     * STATUS - Active status
     * INCOME_AMT - Income classification
     * SPECIAL_CONSIDERATIONS - Special considerations for application
     * ASK_AMT - Funding amount requested
 * Variables removed:
     * EIN - Applicant ID
     * NAME - Name of applicant

 * In my initial model, I chose to create a basic model with two hidden layers and an output layer. The first hidden layer has 80 neurons and the second layer has 30 neurons. Both layers use ReLU as the activation function. The output layer uses sigmoid for the activation function. I chose these numbers because they were basic and knowning I would be adjusting these hyperparameters in the future.

 * The initial model has a performance of 72.47% accuracy which is under the 75% target accuracy,
 * In my optimization attempts, I tried the following:
     * Increasing the number of hidden layers to 3
     * Increasing the number of neurons per layer
     * Increasing the number of epochs to 150

 * Even after all the optimization attempts, the best performance I could achieve was 72.65% accuracy.

3. Overall, it is very difficult to try get past the 72% accuracy hurdle despite the optimization attempts. The charity data requires a deeper understanding in order for more accurate neural network models to be created. I would recommend try breaking up the 'Other' category for the APPLICATION_TYPE column more so the models can try to understand the complexity of the data more. This can allow models to gain a few more points in accuracy.





