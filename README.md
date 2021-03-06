# Real Estate Price Prediction

## Problem Statement

Consider a real estate company that has a dataset containing the prices of different houses  of unit area. The company intends to use this data to creat a system that helps predict the price of housing based on the independent varaisables which includes: housing age, distance to the nearest MRT station, number of convenience stores, latitude and longitude

## Essentially, the company wants —

•	To identify the variables affecting house prices per unit area, 
•	To create a linear model that quantitatively relates house prices with variables such as house age, distance to the nearest MRT station etc
•	To know the accuracy of the model, i.e. how well these variables can predict house prices.

## Business Goal

I am required to model the price of houses of a unit area with the available independent variables. It will be used by the management to understand how exactly the prices vary with the independent variables. They can accordingly manipulate the design of the houses, the business strategy etc. to meet certain price levels. Further, the model will be a good way for management to understand the pricing dynamics of a new market.

## Dataset

This dataset includes  414 rows and 8 columns. It has independent features; house age, distance to the nearest MRT station, numbetr of convenience stores, latitude and longitude. All of these features play a very important roll in our prediction of of house price per unit area (y).

## Data splitting to training and testing model
sklearn.model_selection is the library use to split our data into train and test datasets. 
80% will be training data and 20% testing data

# OLS regression results

![olsregression](https://user-images.githubusercontent.com/63025220/93915840-9880cc00-fcd6-11ea-8566-de75dd47278b.PNG)

The p value of all the features is 00.00 and less than 0.05 which mean all the variables or features are important
The sign of regression coefficient tells you whether there's positive or negative correlation between each independent variable and the dependent variable. Positive coefficient indicates as the value of the independent variable increases, the value of the dependent varaiable also incresases and a negative cofficient indicates as the value of the independent variable increases, the value of the dependent varaiable decreases
R-squared is always between 0-100%

## Risidual analysis of trained data

My R2_Score is above 50% which makes it good

## Error term

![error term](https://user-images.githubusercontent.com/63025220/93920017-902b8f80-fcdc-11ea-99dc-d2c0ec94c578.PNG)

Error term is normally distributed, it indicates the assumption on the linear model is fulfilled

## Making prediction on final score

The table shows the actual value and the predicted value of the test values of y

![Capture1](https://user-images.githubusercontent.com/63025220/93920765-9ff7a380-fcdd-11ea-92e7-b17f3fb4cbd2.PNG)

The graph below shows the plot of the actual vs the predicted values of y-test

![Capture2](https://user-images.githubusercontent.com/63025220/93921380-7d19bf00-fcde-11ea-927b-6799cff97a3d.PNG)

## Evaluating model performance

### MAE = 5.4183854395275235 MSE = 49.41158174311 RMSE = 7.029337219333698




