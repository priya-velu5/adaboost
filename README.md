# adaboost
This is an implementation of the adaboost classifier on heart disease prediction dataset available in: https://www.kaggle.com/ronitf/heart-disease-uci

AdaBoost classifier builds a strong classifier by combining multiple poorly performing classifiers so that you will get high accuracy strong classifier. The basic concept behind Adaboost is to set the weights of classifiers and training the data sample in each iteration such that it ensures the accurate predictions of unusual observations. Any machine learning algorithm can be used as base classifier if it accepts weights on the training set. By default, the Adaboost API from sci-kit learn uses Desition Tree classifier. 

Below are the steps for performing the AdaBoost algorithm:

-> Initially, all observations are given equal weights.

-> A model is built on a subset of data.

-> Using this model, predictions are made on the whole dataset.

-> Errors are calculated by comparing the predictions and actual values.

-> While creating the next model, higher weights are given to the data points which were predicted incorrectly.

-> Weights can be determined using the error value. For instance,the higher the error the more is the weight assigned to the observation.

-> This process is repeated until the error function does not change, or the maximum limit of the number of estimators is reached.



Steps to implement the code:
1. Load the dataset into a dataframe
2. Separate the feature vector and target variable 
3. SPlit the dataset into training set and test set - a 70/30 ratio is ideal
4. Create adaboost classifier object
5. Train the dataset
6. Check the model accuracy 


References :
https://www.kaggle.com/prashant111/adaboost-classifier-tutorial
