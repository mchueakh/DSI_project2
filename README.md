# ![](https://ga-dash.s3.amazonaws.com/production/assets/logo-9f88ae6c9c3871690e33280fcf557f33.png) Project 2 - Ames Housing Data and Kaggle Challenge


## Objectives:
- Predicting the sales price for each house in Ames Housing Data by using linear regression. This also part of Kaggle Challenge in [DSI-US-6 Regression Challenge](https://www.kaggle.com/c/dsi-us-6-project-2-regression-challenge)

### Data Source

- The train.csv and test.csv are on the [DSI-US-6 Regression Challenge Data](https://www.kaggle.com/c/dsi-us-6-project-2-regression-challenge/data)

## The Workflow Process

### 0. Define problem
- What are the properties of house that make the house get the good selling price? such as size of area, car area, number of Bedroom etc. 
- The purpose of this study is a guideline for house agency staffs to find the high price house and get more commission.

### 1. Data Preparation
- Load data dictionary from 'http://jse.amstat.org/v19n3/decock/DataDocumentation.txt'
- Mapping column name from data dict and Data source
- Replace the null values by proper values based on data dict type [ numerical or category ]
- Convert the category values in Ordinal cols to be the scale discreate values

### 2. EDA and Feature Engineering
- Encode the category cols by using OneHotEncoder
- normalization by using StandardScaler

### 3. Get pre-predictors from correlation between features and target 
- Get Cols which have the high correlation with target (SalePrice)

### 4. First Liner Regression Model 
- Create X_train from pre-predictos list
- Split data to X,y Train and Test
- Evaluate the model

### 5. Perform Regularization (Lasso) to get Optimal Predictors
- get the best Lasso alpha for Training data
- remove features which have coeffienct equal to zero from the pre-predictos list, get the optimal-predictor list

### 6.Optimal Liner Regression Model by using Optimal Predictors
- Create X_train from optimal-predictos list
- Evaluate the model

### 7. Get prediction result from X_test and run Kaggle Challenge



## Conclusion


Top three features that make the house get a better price are:

1. Size of the Ground living area
    * every one square feet step up, the price increase about 24,633 US dollar 


2. Rates of the overall material quality
    * every one rate step up, the price increase about 18,854 US dollar


3. Size of basement area
    * every one square feet step up, the price increase about 14,928 US dollar
    
#### House agency staffs should focus on house that has big groud living and basement area and also good material quality then they get high commision. 
