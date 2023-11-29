# parkinsons
Parkinson's Telemonitoring Score Estimation


This project was aimed at developing a ML algorithm to estimate UPDRS score based on a training set and testing it on a test set. Many regression ML models were used including Linear Regression, Ridge Regression, Lasso Regression, LassoCV Regression, Elastic Regression, KNN Regression, Decision Tree Regression, LinearSVR Regression, and finally RandomForest Regression. The RandomForest regression provided the highest R^2 score of 0.8909 with a MAE of 2.25 and mean value of 29.35. The most important features were identified to be age, DFA signal, and sex. These also correspond to real life facts about Parkinson's disease and make sense. The least important features were Shimmer:APQ3, Shimmer, and Jitter:RAP. These were dropped from the ML model and saw a very slight but insignificant increase in accuracy. Test_time was also dropped because it was not random data and not relevant to pattern prediction. As per the project instructions motor_UPDRS was also dropped because this was a physician's estimation and not relevant to our experiment. Thus the RandomForest regression model was selected as the most accurate with n_estimators = 100 with the default depth. Pycaret was also run and the results corresponded with the findings of this project of RandomForest being among the best regressors for this experiment.

Video Demo:
https://youtu.be/WBQJNfvlFjo
