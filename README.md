# Bike-Sharing-Demand-Prediction

Currently Rental bikes are introduced in many urban cities for the enhancement of mobility comfort.Rental bike sharing system is a shared transport service in which bicycles are made available for shared use to individuals on a short-term basis for a price. It is becoming popular because of increased comfortableness and environmental sustainability. Eventually, providing the city with a stable supply of rental bikes becomes a major concern. The crucial part is the prediction of bike count required at each hour for the stable supply of rental bikes. Our project is about making a predictive model which can help in predicting bike count required at each hour.

## Problem Statement
It is important to make the rental bike available and accessible to the public at the right time as it lessens the waiting time. This project tackles the problem of predicting the number of bikes which will be rented at any given hour in a given city. The main objective is to build various regression models and analyze their performance with respect to each other so as to get the best performing model, which could help in predicting the number of bikes required at each hour for the stable supply of rental bikes.

## Data Overview
For our project, we are provided with the Seoul Bike sharing demand dataset. The dataset contains per day Bike Rental Count with 8760 entries, possessing 14 attributes, out of which 13 variables are independent and one dependent form the part of our Regression Analysis. The dataset contains weather information (Temperature, Humidity, Windspeed, Visibility, Dewpoint, Solar radiation, Snowfall, Rainfall), the number of bikes rented per hour and date information. The time span of the dataset is 365 days from December 2017 to November 2018. From the data, the count of the rental bikes rented at each hour is calculated.

## Methodology
![Screenshot (133)](https://user-images.githubusercontent.com/82964400/151691046-bbed0634-1f32-4f20-b469-d26bf938e0f9.png)

Our project consists of four phases namely- Data exploration, Data analysis, Data preparation and building models and analyzing their performance using various evaluation metrics.

For modeling we tried various regression models such as-
1)Linear Regression	      

2)Lasso Regression

3)Ridge Regression	     

4)Elastic Net

5)Decision Tree	          

6)Random Forest

7)Gradient Boosting	      

8)XGBoost Regressor	

All these models were fine tuned using a grid search method with repeated cross-validation (CV) to ﬁnd the best hyperparameters. We have also plotted variable importance plots for tree based models to determine the features that were most important while model building.

## Results

After training the models with their best hyperparameters, the performance of each of the regression models were evaluated using the testing set with evaluation metrics.  The model which provides the highest R2 values and lowest MSE, RMSE and MAE is the best one.

![res](https://user-images.githubusercontent.com/82964400/151691674-23b5ce18-ea09-4481-bde0-05c0b4d41224.png)

## Conclusion

* There is a huge demand for bike rents in the summer season while the least bike rents occur in winter.
* The demand for rental bikes is at peak at 8am and 6pm so we can say that demand is more during office opening and closing time.
* Temperature and hour are the most influential features to predict the rental bike count.
* Gradient Boosting and XGBoost models are found to be the best models.
* Therefore, either Gradient Boosting or XGBoost model can be used to predict the number of bikes required at each hour.

