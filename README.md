# Neural_Network_Charity_Analysis by Ketaki
## Overview of the analysis: Explain the purpose of this analysis.
This project helps our user, Beks to predict if applicants to AlphabetSoup, a charitable organization, will be successful if funded by them. This is done by creating a binary classifier using Neural Networks on a history [Dataset]() that have received funding from AlphabetSoup. This dataset is first pre-processed using Pandas libraries, then the Neural network model is complied and trained and finally tested to check it's accuracy. To achieve a desired level of accuracy, we also optimize the model by altering the input parameters, adding more hidden layers to the mdoel, using different algorithms, etc.

## Results: Using bulleted lists and images to support your answers, address the following questions.

Data Preprocessing
What variable(s) are considered the target(s) for your model? 
 The target variable for the dataset is the **IS_SUCCESSFUL** column of the csv file. 
What variable(s) are considered to be the features for your model?
- The feautues of the model were -
- APPLICATION_TYPE—Alphabet Soup application type
- AFFILIATION—Affiliated sector of industry
- CLASSIFICATION—Government organization classification
- USE_CASE—Use case for funding
- ORGANIZATION—Organization type
- STATUS—Active status
- INCOME_AMT—Income classification
- SPECIAL_CONSIDERATIONS—Special consideration for application
- ASK_AMT—Funding amount requested

What variable(s) are neither targets nor features, and should be removed from the input data?
- Variables such as EIN and NAME were not considered as targets or features as they do not assist in characterizing the output of the dataset.
Compiling, Training, and Evaluating the Model
How many neurons, layers, and activation functions did you select for your neural network model, and why?
- Depending on the input parameters of 43, the number of neurons used were 80 for the input layer which was roughly twice the number of inputs. 
Were you able to achieve the target model performance?
- The achieved target performance was ~74% with the optimizations.
What steps did you take to try and increase model performance?
- Attempt #1
- Attempt #2
- Attempt #3

## Summary: Summarize the overall results of the deep learning model. Include a recommendation for how a different model could solve this classification problem, and explain your recommendation.
- We overall achieved an accuracy of ~74% which was a little less compared to the desired accuracy of 75%.
- Even with optimization, it was a challenge to achieve the desired accuracy. This was probably because of overfitting of the data by the model.
- Recommendation - We can use other supervised machine learning algorithms such as the Random Forest Classifier Algorithm to achieve the desired accuracy. As shown, we can get the desired level of accuracy with Random Forest Classifier.
