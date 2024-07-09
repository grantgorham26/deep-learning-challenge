# deep-learning-challenge

## Report

### Overview
The purpose of this analysis was to create and train a mchine lerning model and neural network that would be able to accurately predict whether applicants will be successful if funded by alphabet soup. 


### Results
* Data Preprocessing
  - The target variable for the model I created was whether the organizaton was sucesfull from alphabet soup funding. On the image of the dataframe below it is boxed in red. 
  - The variables that were feautures for the first implementation of the model were APPLICATION_TYPE, AFFILIATION, CLASSIFICATION, USE_CASE, ORGANIZATION, STATUS, INCOME_AMT, SPECIAL_CONSIDERATIONS, and ASK_AMT. These features were then split into more features using pd.get_dummies when training and fitting the model. During optimization i also dropped a few of the features in attempt to increase the accuracy. In the image below I have boxed the feature variables in green. 
  - Variables that needed to be dropped from the orginal data included the EIN and Organization Name. These were dropped because they could not be a target or a feature because they just identify the organization. In the image below i have box the identifier variables in blue.
 
 ![Screenshot 2024-07-09 at 1 22 52 PM](https://github.com/grantgorham26/deep-learning-challenge/assets/154031840/83bf8a30-2aec-4fdb-be1a-224526e0578d)


### Summary 
 
