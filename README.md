# Project Name


## Table of Contents
* [General Info](#general-information)
* [Technologies Used](#technologies-used)
* [Conclusions](#conclusions)


<!-- You can include any other section that is pertinent to your problem -->

## General Information
A US-based housing company named <b>Surprise Housing</b> has decided to enter the Australian market. The company uses data analytics to purchase houses at a price below their actual values and flip them on at a higher price. For the same purpose, the company has collected a data set from the sale of houses in Australia.

 

The company is looking at prospective properties to buy to enter the market. You are required to build a regression model using regularisation in order to predict the actual value of the prospective properties and decide whether to invest in them or not.

 + ### Business Goals

You are required to model the price of houses with the available independent variables. This model will then be used by the management to understand how exactly the prices vary with the variables. They can accordingly manipulate the strategy of the firm and concentrate on areas that will yield high returns. Further, the model will be a good way for management to understand the pricing dynamics of a new market.<hr>

The company wants to know:
- Which variables are significant in predicting the price of a house, and
- How well those variables describe the price of a house.

Also, determine the optimal value of lambda for ridge and lasso regression.

## Conclusions
From our research,<br>
we noticed that Simple Linear Regression did not provide us with a satisfactory model. <br>
<br><br>However,<br> With the help of other regression techniques, we can come to passable conclusions.<br><br>
Both Ridge and Lasso Regression techniques provide us with models that describe the trends in the dataset fairly well.

> <b>Ridge</b> regression gives us an $R^2$ Value of $0.91$ and $0.90$ at $\lambda = 5$ and, <br> 
> <b>Lasso</b> Regression gives us an $R^2$ Value of $0.92$ and $0.88$ at $\lambda = 100$<br> 
> for train and test data respectively
<br>

It would seem that Ridge regression slightly surpasses Lasso regression only because it performs marginally better on the unseen/test data, however, Lasso regression does eliminate several variables and simplifies the model. <br> Yet, both models perform relatively well. It will come down to the business requirements to decide which model can be used. 
<br><br>
As far as the Business requirements go, Ridge regression suggests using the variables : 

1. `GrLivArea`    : Above grade (ground) living area square feet
2. `OverallQual`  : Rates the overall material and finish of the house
3. `2ndFlrSF`     : Second floor square feet
4. `1stFlrSF`     : First Floor square feet
5. `TotalBsmtSF`  : Total square feet of basement area

With 259 variable model complexity
<br><br>
And Lasso Regression considers using the variables:

1. `GrLivArea` : Above grade (ground) living area square feet
2. `TotalBsmtSF` : Total square feet of basement area
3. `OverallQual` : Rates the overall material and finish of the house
4. `RoofMatl_WdShngl` : If the roof materials consists of Wood Shingles
5. `2ndFlrSF` : Second floor square feet

With 157 variable model complexity


## Technologies Used (libraries)
- numpy
- pandas
- matplotlib
- seaborn
- sklearn
- statsmodels
- warnings
