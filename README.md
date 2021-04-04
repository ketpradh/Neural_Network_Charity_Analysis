# Neural_Network_Charity_Analysis by Ketaki
## Overview of the analysis: Explain the purpose of this analysis.
This project helps our user, Beks to predict if applicants to AlphabetSoup, a charitable organization, will be successful if funded by them. This is done by creating a binary classifier using Neural Networks on a history [Dataset](https://github.com/ketpradh/Neural_Network_Charity_Analysis/blob/main/Resources/charity_data.csv) that have received funding from AlphabetSoup. This dataset is first pre-processed using Pandas libraries, then the Neural network model is complied and trained and finally tested to check it's accuracy. To achieve a desired level of accuracy, we also optimize the model by altering the input parameters, adding more hidden layers to the mdoel, using different algorithms, etc.

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

- Variables such as **EIN and NAME** were not considered as targets or features as they do not assist in characterizing the output of the dataset.
- Depending on the input parameters of 43, the number of neurons used were 80 for the input layer which was roughly twice the number of inputs. 
- The achieved target performance was ~72.6% without the optimizations.
- **Attempt #1 Change the Activation Functions**
- ![Parameters](https://github.com/ketpradh/Neural_Network_Charity_Analysis/blob/main/Resources/Attempt%201%20-%20Params.PNG)
- ![Results](https://github.com/ketpradh/Neural_Network_Charity_Analysis/blob/main/Resources/Attempt%201%20-%20Accuracy.PNG)
- **Attempt #2 Change the number of neurons in the hidden layers and increase number of epochs**
- ![Parameters](https://github.com/ketpradh/Neural_Network_Charity_Analysis/blob/main/Resources/Attempt%202%20-%20Params.PNG)
- ![Results](https://github.com/ketpradh/Neural_Network_Charity_Analysis/blob/main/Resources/Attempt%202%20-%20Accuracy.PNG)
- **Attempt #3 Add an additional hidden layer**
- ![Parameters](https://github.com/ketpradh/Neural_Network_Charity_Analysis/blob/main/Resources/Attempt%203-%20Params.PNG)
- ![Results](https://github.com/ketpradh/Neural_Network_Charity_Analysis/blob/main/Resources/Attempt%203%20-%20Accuracy.PNG)
- However, even with optimizations, the desired performance was not achieved.

## Summary: 
- We overall achieved an accuracy of ~74% which was a little less compared to the desired accuracy of 75%.
- Even with optimization, it was a challenge to achieve the desired accuracy. This was probably because of overfitting of the data by the model.
- Recommendation - We can use other supervised machine learning algorithms such as the Random Forest Classifier Algorithm to achieve the desired accuracy. As shown, we can get the desired level of accuracy with Random Forest Classifier.
