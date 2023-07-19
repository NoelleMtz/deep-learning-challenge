# deep-learning-challenge
Deep learning challenge- Module 21 for UofA Data Analytics Bootcamp 2023

# Authors
Noelle G Martinez

# Background
The nonprofit foundation Alphabet Soup wants a tool that can help it select the applicants for funding with the best chance of success in their ventures. With your knowledge of machine learning and neural networks, you’ll use the features in the provided dataset to create a binary classifier that can predict whether applicants will be successful if funded by Alphabet Soup.

From Alphabet Soup’s business team, you have received a CSV containing more than 34,000 organizations that have received funding from Alphabet Soup over the years. Within this dataset are a number of columns that capture metadata about each organization...

# Report
## Overview
The purpose of the analysis is to determine whether applicants will be successful if funded by Alphabet Soup.

## Results
*	Data Preprocessing
    *	_What variable(s) are the target(s) for your model?_ IS_SUCCESSFUL
    *	_What variable(s) are the features for your model?_ 'APPLICATION_TYPE', 'AFFILIATION', 'CLASSIFICATION', 'USE_CASE', 'ORGANIZATION', 'STATUS', 'INCOME_AMT', 'SPECIAL_CONSIDERATIONS', 'ASK_AMT'. Addded back ‘NAME’ for the optimized model, especially because some companies have reapplied many times.
    * _What variable(s) should be removed from the input data because they are neither targets nor features?_ EIN

* Compiling, Training, and Evaluating the Model
  *  _How many neurons, layers, and activation functions did you select for your neural network model, and why?_
   I used Rectified Linear Unit (ReLU) and Sigmoid. I used 2 hidden layers and their corresponding nodes were 10 and 5, respectively. I chose these numbers initially because they seemed like round numbers. I did not change the layers or nodes because once I added the NAMES variable, things ran fine.
  ![Picture1](https://github.com/NoelleMtz/deep-learning-challenge/assets/123044294/51700768-8a7e-4bd1-9587-0addae1a5593)

  * _Were you able to achieve the target model performance?_ Initially, not without the ‘NAMES’ variable. But after re-adding it, I was able to reach 79 % accuracy.
  
    ![Picture2](https://github.com/NoelleMtz/deep-learning-challenge/assets/123044294/38cd1f3f-a0e2-42df-9801-782b44225e07)

  * _What steps did you take in your attempts to increase model performance?_ Tried adding back a dropped variable. And ‘NAMES’ were the company names that applied. Some of the companies had counts over 500, which means that they applied multiple times. This could add the success of the application.

## Summary
By including ‘NAMES’ variable, the optimized model can predict the success of applicants with 79% accuracy. Another model that could solve this problem would be to add more 


# References
IRS. Tax Exempt Organization Search Bulk Data Downloads. https://www.irs.gov/
