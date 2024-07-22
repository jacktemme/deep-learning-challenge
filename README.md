# Alphabet Soup Charity Report 

## Overview of the Analysis
This repository employs a neural network model from the Tensor Flow library to help the nonprofit organzation Alphabet Soup determine how likely an applicant that requests funding will be successful in their venture. The model is trained on 80% of the data, and features are based off of a variety of determining factors of the applicant such as, income amount, ask amount, affiliation, etc. The remaining 20% of the data is used to evaluate the model's performance by comparing predicted success outcomes with the actual results. The overall goal of this model is to help this non profit better assess the potential risks of approving funding for an application and therefore allowing the company to make more informed decisions with their money allocation.

## Results

### Data Preprocessing
* The target of this data set was the binary classification on whether the funding for the application was deemed successful. 
* The features of the data that the neural network was trained on was the Affiliation, Classification, Organization, Use, Status, Income Amount, Ask Amount and Special Considerations of the applicant.
* The Name and EIN number from the data were dropped as they only differentiate the applicant would not impact the outcome of the applicants success.

### Compiling, Training, and Evaluating the Model

* For my neural network model two hidden layers were used with the relu activation function. 30 neurons were in the first layer, followed by 15 in the next layer. The final output layer used a singular neuron with a sigmoid activation function to correctly output a binary classification for this model.
* The neural network model had a accuracy of 73.04% when used on the testing data, which was close, but not able to achieve the desired target of 75% accuracy. Therefore, the model is on the right track but more fine tuning would need to be done to create more accurate outputs.
* In order to slightly increase the output of this model, the activation function was changed to a relu instead of tanh in the hidden layers and the number of neurons and epochs were decreased. 


## Summary

Overall, this neural network model was close to reaching Alphabet Soup's target of 75% accuracy in determining the success outcome when funding an applicant, but still fell short. The fact that decreasing neurons and epochs of this model increased accuracy suggests that the model had a tendency to overfit the data. This is likely because the model trained intensively on the outliers and noise in the data, becoming less accurate at the overall classification of the applicant's success. Therefore, the best way to create a more accurate model would be to more intensively process the data before running it through the neural network. The data has lot of features for the applicant and some might impact the outcome more than others. So it could be beneficial to use a principal component analysis to reduce the noise of the data and hopefully help the model make more accurate predictions. 


