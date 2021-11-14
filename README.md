# water_potability_predictor
*  Potability of water indicates if water is safe for human consumption. Here, 1 = Potable and 0 = Not Potable
*  My goal in this project was to compare several classification models to find the one that predicts the potability of water with highest accuracy and lowest False Positves
*  The classification models I compared were Extreme Gradient Boosting (XGBoost), Gradient Boosting (GBoost), Random Forest, and K Nearest Neighbors (KNN)
*  I used SciKit learn's *GridSearchCV* to perform the hyperparameter tuning
*  The dataset was obtained from kaggle.com and contains nine water quality metrics for 3276 different water
*  **XGBoost** model can predict the water potability with accuracy score of **79%**. Below is the plot of the Confusion Matrix for the XGBoost model
*  **Random Forest** model can predict the water potability with accuracy score of **78%**. Below is the plot of the Confusion Matrix for the Random Forest model
*  **Gradient Boosting** model can predict the water potability with accuracy score of **80%**. Below is the plot of the Confusion Matrix for the Gradient Boosting model
*  **KNN** model can predict the water potability with accuracy score of **63%**. Below is the plot of the Confusion Matrix for the KNN model
*  The Gradient Boosting model is the best not only because it has the highest accuracy but has the lowest false positives percentage.
*  Because a false poisitive by this will be very catastrophic, I will select the model with lowest percentage of false positive and highest recall score.  Therefore, **Gradient Boosting** wins!
*  A plot of feature importance from the Gradient Boost model is shown below
*  The sulfate concentration and pH are the top two most important features in determining the potability
