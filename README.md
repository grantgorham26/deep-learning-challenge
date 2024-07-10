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
When looking at how the models scored in accuracy the third optimization was the best, followed by the first model, then the second optimization attempt and the least accurate was the first optimization attempt. In terms of the loss all the models were about the same ranging from .5601 to .5623. 

first model scores:
![Screenshot 2024-07-09 at 3 53 44 PM](https://github.com/grantgorham26/deep-learning-challenge/assets/154031840/b905f461-6edf-4a55-8df2-f5e095897e15)




first optimization attempt scores:
![Screenshot 2024-07-09 at 3 53 53 PM](https://github.com/grantgorham26/deep-learning-challenge/assets/154031840/b83fc66b-7a59-4bc8-bb19-1a1bc6f3201f)



second optimization attempt scores:
![Screenshot 2024-07-09 at 3 54 06 PM](https://github.com/grantgorham26/deep-learning-challenge/assets/154031840/77508997-6dd0-4bd7-ace5-2e67c839c9c9)




third optimization attempt scores:
![Screenshot 2024-07-09 at 3 54 14 PM](https://github.com/grantgorham26/deep-learning-challenge/assets/154031840/7a0a8318-6966-4d62-beb4-215d502f8188)

 
