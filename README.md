# Neural Network Charity Analysis

## Purpose of this Analysis

The purpose of this analysis was to assist Beks in creating neural networks that can predict whether applicants will be successful if funded by Alphabet Soup.

## Results

### Data Preprocessing

#### What variable(s) are considered the target(s) for your model?

The target variable for our model is: IS_SUCCESSFUL

#### What variable(s) are considered to be the features for your model?

The features of this model are as follows:
'APPLICATION_TYPE',
 'AFFILIATION',
 'CLASSIFICATION',
 'USE_CASE',
 'ORGANIZATION',
 'INCOME_AMT',
 'SPECIAL_CONSIDERATIONS'

#### What variable(s) are neither targets nor features, and should be removed from the input data?

The variables “Name” and “EIN” were removed from our input data as we deemed them not applicable to success of Alphabet Soup’s funding model and analysis.

### Compiling, Training, and Evaluating the Model

#### How many neurons, layers, and activation functions did you select for your neural network model, and why?

Attempt 1 – I started with 2 hidden layers with 100 neurons and 50 neurons, run with 100 epochs. The neurons are an increase from deliverable 2. I used this attempt as a benchmark so that I could adjust the subsequent attempts. Accuracy was 70.2%.
![Alt Text](https://github.com/lauren1478/Neural_Network_Charity_Analysis/blob/main/Supporting%20PNGs/Attempt%201.png)

Attempt 2 – I chose to add another hidden layer for a total of three hidden layers with 100 epochs. With the addition of the 3rd hidden layer I chose 25 neurons. Accuracy was 68.4%.
![Alt Text](https://github.com/lauren1478/Neural_Network_Charity_Analysis/blob/main/Supporting%20PNGs/Attempt%202.png)

Attempt 3 – I decided to remove the 3rd hidden layer as the last attempt produced a lower accuracy than attempt one. Instead, I increased the epochs and ran it through 200 epochs. Accuracy was 67%
![Alt Text](https://github.com/lauren1478/Neural_Network_Charity_Analysis/blob/main/Supporting%20PNGs/Attempt%203.png)

#### Were you able to achieve the target model performance?

I did not achieve the target model performance after 3 attempts. The highest accuracy I was able to achieve was 70.2% (attempt 1) and the lowest was 67% (attempt 3).

#### What steps did you take to try and increase model performance?

Attempt 1 – Increased the numbers of nuerons in each layer

Attempt 2 – Added a third hidden layer 

Attempt 3 – Removed the third hidden layer and increased the number of epochs.

## Summary

Overall, we were not able to achieve the 75% accuracy rate, however we were very close with attempt number 1. The other attempts, though lower in accuracy, only decreased by a small magnitutude. With additional tweaks to the code, we could get even closer to the 75% accuracy. Because of the large number of rows and the small amount of features, we could try a supervised learning model such as a Random Forest model.
