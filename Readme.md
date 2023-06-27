## Introduction
Fall detection is a subset of a broader category of problems called "Human Activity Recognition" (HAR). HAR is a classification problem where the goal is to classify the activity being performed by a person. The activities can consist of walking, sitting, standing, running etc. Fall detection is a subset of HAR where the goal is to classify the activity as a fall or not.

## Problem Statement
To detect, using smartphone sensor data, when a person has fallen. This is a binary classification problem where the goal is to classify the activity as a fall or not.

## Data
We are using the K-Fall as well as the UMass Dataset (both of which are available upon request from their respective research groups). The data is then cleaned and processed to work nicely with the models we are using. The data is then split into training and testing sets. The training set is used to train the model and the testing set is used to evaluate the model.

## Models
We found that a Convolutional Neural Net (CNN) works best for this problem. We also tried a Long Short Term Memory (LSTM) model but it did not perform as well as the CNN. The CNN model is trained on the training set and then evaluated on the testing set. The model is then saved and can be used to make predictions on new data.
It averages around 94% accuracy on the testing set.