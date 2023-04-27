# Neural Network Charity Analysis
## Analysis
This challenge is about helping a co-worker to use machine learning and neural networks to create a binary classifier.  This classifier uses features in the provided dataset that is capable of predicting whether applicants will be successful if funded by the hypothetical company that is considering investments.  The file includes more than 30,000 organizations with many different relevant data points as well as their success rates from the past that will be used to predict future success.

## Results:

### Data Preprocessing
* **What variable(s) are considered the target(s) for your model?**
The target for the model is the column telling whether the investment was successful or not, the "IS SUCCESSFUL" column, as it is the variable that we are testing and training for.
* **What variable(s) are considered to be the features for your model?**
The features are the variables that we use to measure the target, which include 'APPLICATION_TYPE', 'AFFILIATION', 'CLASSIFICATION', 'USE_CASE', 'ORGANIZATION', 'INCOME_AMT',and 'SPECIAL_CONSIDERATIONS,' as these are used to predict the success when we train and test the model.
* **What variable(s) are neither targets nor features, and should be removed from the input data**
The variables that could be dropped were the NAME and EIN columns as they were string values that only served as name identifiers for the data and did not provide relevant information for the data.
### Compiling, Training, and Evaluating the Model
* **How many neurons, layers, and activation functions did you select for your neural network model, and why?**
My initial model ran two layers with 100 neurons, using three different activation functions.  I wanted to keep the model simple at first as the lessons warned about too many neurons and hidden layers can overfit the testing data and thus be less accurate.
* **Were you able to achieve the target model performance?**
No, my model was able to consistently run with about 72% accuracy, just shy of the desired 75% accuracy.
* **What steps did you take to try and increase model performance?**
In the end I added four total layers to my model with 151 neurons.  I used three different activation functions.  It was mostly trial and error as I was trying to improve the results of my model that these decisions were made.
![model description](https://github.com/machudpicchu/Neural_Network_Charity_Analysis/blob/main/Layer_Description.png)
## Summary:
In the end, the model was able to run with around a 72% accuracy for predicting the likelihood of a successful investment.  
![Model Results](https://github.com/machudpicchu/Neural_Network_Charity_Analysis/blob/main/Results_Optimized.png)

If I were to run this model again, I would recommend a Random Forest as a means to make predictions as it has a higher probability of being accurate.
