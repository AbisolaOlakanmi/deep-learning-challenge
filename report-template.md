# Module 21 Report 

## Overview of the Analysis

Using machine learning and neural networks to create a binary classifier that can predict whether applicants will be successful if funded by Alphabet Soup.
The dataset contains more than 34,000 organizations, including metadata such as application type, affiliated sector of industry, government organization classification, use case for funding, income classification, funding amount requested, and whether the money was used effectively. The analysis involves preprocessing the dataset by dropping unnecessary columns, encoding categorical variables, and splitting the data into training and testing datasets. The neural network model is then designed, trained, and evaluated to determine its loss and accuracy. Lastly, the model is optimized using various methods such as adjusting input data, adding more neurons and hidden layers, using different activation functions, and adjusting the number of epochs. The ultimate goal is to achieve a predictive accuracy higher than 75% and save the optimized model as an HDF5 file.



## Results

Data Prepocessing

- What variable(s) are the target(s) for your model?
The target variable(s) for the model is IS_SUCCESSFUL, it represents the binary classification outcome variable of whether a charity donation was successful or not.

- What variable(s) are the feature(s) for your model?
The feature variables for the model are all the other columns in the DataFrame, excluding IS_SUCCESSFUL.

- What variable(s) should be removed from the input data because they are neither targets nor features?

As part of the preprocessing phase for the analysis, I have identified that the EIN or Employee Identification Number does not contain relevant information for our predictive model. As such, I excluded this variable from the feature and target selection, as it is not pertinent to the analysis.
