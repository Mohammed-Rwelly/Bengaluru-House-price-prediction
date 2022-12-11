# Bengaluru-House-price-prediction
The objective of the project is to create a Machine Learning Model .We are doing a supervised learning and our aim is to do predictive analysis to predict housing price
In this project, we will implement a Bangalore House Price Prediction model using a Machine Learning algorithm. This model predicts the price of Bangalore's house with the help of a few parameters like availability, size, total square feet, bath, location, etc. 

# Steps of project :

#### Wrangling:

All the columns with Null data points were dropped. Inconsistency in location, total_sqft and size columns were also handled by writing appropriate functions.

#### Feature Engineering: 

Some additional features like ‘price_per_sqft’ were created that helped me in filtering out outliers.

#### Dimensionality Reduction: 

In location many places had only one data point. This could lead to a lot of independent variables for the ML model. Any location with more than 10 data points were clubbed together.

#### Outlier detection: 

Outlier detection phase, some outliers were removed just by doing preliminary exploration, some were removed using respective mean and standard deviation.

#### One hot encoding:

One hot encoding was used for managing categorical data which was location for me in this project

#### K fold Cross validation:

Shuffle split with 10 folds with cross_val_score was used to check the performance of our regression model.

#### GridSearchCV: 

GridSearchCV was used for choosing the best algorithm amongst lasso, Decision Tress regressor ,linear regression  and xgbregressor. It is also used for Hyper parameter tunning for the best algorithm, and ﬁnally gone linear regressor the best  with 0.84

![image](https://user-images.githubusercontent.com/46110270/206910352-70d24b86-efeb-43a0-9601-fe3d8b0af794.png)


#### Major Python Libraries use:
sklearn, pandas, numpy , matplotlib , cross_val_score, GridSearchCV
