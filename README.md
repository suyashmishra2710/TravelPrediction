# TravelPrediction

## About 
This project uses survey data indicating passenger satisfaction with different U.S. airlines. The purpose of this project was to identify features relating specifically to the flight that could be used to make classification models predicting whether or not a passenger would be satisfied by their air travel experience. From the dataset, the different aspects users rated from 0-5 on satisfaction include seat comfort, departure/arrival time convenient, food and drink, gate location, inflight wifi service, inflight entertainment, online support, ease of online booking, on-board service, leg room service, baggage handling, checkin service, cleanliness, and online boarding. There were other factors in the dataset (i.e. departure delay in minutes, age, flight distance, etc.), but those weren’t used as the purpose of the task was to understand the individual aspects relating to the flight itself and see if that could be used to predict passenger satisfaction. The expected output from these classification models is an output array with two different values: satisfied and neutral/dissatisfied. Given that this dataset also had a column indicating whether passengers were satisfied or neutral/dissatisfied, the output of the classification models were compared with these ground truth values and a classification report detailing accuracy, recall, precision, and f1-score was displayed for all classification algorithms used.

## Methodology
In this project, three different classification models were used: a decision tree, K-nearest neighbours, and support vector machines. The results of the models were comparable with SVM performing slightly better than the other two. 

To prepare the data, the following steps were taken: 
1) Low variance threshold was applied to remove features where more than 20 percent of its values were missing.
2) Mutual information scores between various featues and the target variable were computed to determine how much uncertainty in the target variable was reduced when a feature took on a specific value.
3) The three different models were trained using various sklearn functions. 
