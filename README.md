# Food-sales
Jonathan Hernandez

The goal of this analysis is to provide insights into the stores sales data and to create machine learning model that predicts a variation in the data.

# Data Dictionary 
![image](https://user-images.githubusercontent.com/127071673/230613170-e99a6001-6f3a-4519-a8a4-47f9318531bc.png)

# Data Cleaning
Before the machine learning preprocessing, the date was cleaned using these steps

- Any spelling inconsistencies 
- Any duplicates were dropped
- Categorical ordinal data was numerically encoded
-High-cardinality feature was dropped ('Item_Identifier')

# Exploratory Visuals 

To understand the data, I created some visual models.

The first visual consist of Count of items vs the Weight of them
![image](https://user-images.githubusercontent.com/127071673/230614342-108a4a25-c6fa-457e-8b65-458f3cfcf94a.png)

The second visual consist of a heat map which shows the correlation coefficient between each of the numeric variables. This
is a good way to see a visual of their relationships.

![image](https://user-images.githubusercontent.com/127071673/230615807-26d97d9b-1b2f-4218-a612-b6a53afc4ce4.png)

* What is the relationship between the item type and sale? 

![image](https://user-images.githubusercontent.com/127071673/230616362-335695de-b5c3-4d53-a6c1-0efec14cb676.png)

#What is the correlation between sales and the products size?

![image](https://user-images.githubusercontent.com/127071673/230616915-e6dbd35d-751d-400a-9200-616e64493228.png)

The scatterplot indicates a positive correlation within the price and sales of items. The more products sold the more money comes in. The more expensive the item is the less amount of that particular is sold.

# Machine Learning Preprocessing

Missing nominal vlues were imputed with the most frequent value
Nominal features were one-hot encoded
Missing numerical values were imputed with the mean
Numerical features were scaled

# Machine Learning Model: Linear Regression

A linear regression model was fit on the training data which was then tested. Linear Regression
model can account for 57% of the variation in tbe test using the features available. The R/2 was within the range of 1093 dollars.


#Machine Learning Model: Random Forest Regression
A Random Forest model was fit on the training data then tested after.

The random forest regression model was able to account for an average of 55% The R/2 was within the range of 427.

*Recommendation

For the two models linear regression and random forest models, linear random forests model gets closer to predict correctly.

The linear regression model can account an average of 57% of the variation in the test data using the features available. $ 1139 is the average target item outlet.

In Random forests model 93% of the variation can be accounted for using the features available. $427 is the average target item outlet.



