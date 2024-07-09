# deep-learning-challenge

## Report

### Overview
The purpose of this analysis was to create and train a machine learning model and neural network that would be able to accurately predict whether applicants will be successful if funded by alphabet soup. 


### Results
* Data Preprocessing
  - The target variable for the model I created was whether the organization was sucessfull from alphabet soup funding. On the image of the dataframe below it is boxed in red. 
  - The variables that were features for the first implementation of the model were APPLICATION_TYPE, AFFILIATION, CLASSIFICATION, USE_CASE, ORGANIZATION, STATUS, INCOME_AMT, SPECIAL_CONSIDERATIONS, and ASK_AMT. These features were then split into more features using pd.get_dummies when training and fitting the model. During optimization i also dropped a few of the features in attempt to increase the accuracy. In the image below I have boxed the feature variables in green. 
  - Variables that needed to be dropped from the original data included the EIN and Organization Name. These were dropped because they could not be a target or a feature because they just identify the organization. In the image below i have box the identifier variables in blue.
 
 ![Screenshot 2024-07-09 at 1 22 52 PM](https://github.com/grantgorham26/deep-learning-challenge/assets/154031840/83bf8a30-2aec-4fdb-be1a-224526e0578d)
* Compiling, Training, and Evaluating The Model
  - In the first implementation of the model there was 7 neurons used, 2 hidden layers, and i used Relu for the hidden layer activation function and sigmoid for the output layer. I chose sigmoid for the activation function of the output layer because it is a binary classification problem. I used relu for the hidden layers because thats what is most widely used in neural network model hidden layers. 
  - I was unable to achieve the target performance using my first model and the three attempts I made at optimizing it. 
  - In my first attempt at optimization I increase the number of neurons in both hidden layers. In my second attempt I added an extra hidden layer. In my third attempt I added 2 extra hidden layers and adjusted the units in the hidden layers, increased the number epochs to 100 and dropped 3 columns from the dataframe. 


### Summary 


first model scores:




first optimization attempt scores:



second optimization attempt scores:




third optimization attempt scores:

 
