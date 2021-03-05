# ![](https://ga-dash.s3.amazonaws.com/production/assets/logo-9f88ae6c9c3871690e33280fcf557f33.png) Project 2 - Ames Housing Data and Kaggle Challenge


### Objectives:
- Predicting the sales price for each house in Ames Housing Data by using linear regression. This also part of Kaggle Challenge in [DSI-US-6 Regression Challenge](https://www.kaggle.com/c/dsi-us-6-project-2-regression-challenge)

### Data Source

- The train.csv and test.csv are on the [DSI-US-6 Regression Challenge Data](https://www.kaggle.com/c/dsi-us-6-project-2-regression-challenge/data)

## The Workflow Process

### 0. Define problem
**Problem Statement**
- Is it clear what the student plans to do?
- What type of model will be developed?
- How will success be evaluated?
- Is the scope of the project appropriate?
- Is it clear who cares about this or why this is important to investigate?
- Does the student consider the audience and the primary and secondary stakeholders?

### 1. Data Preparation
- Load data dictionary from 'http://jse.amstat.org/v19n3/decock/DataDocumentation.txt'
- Mapping column name from data dict and Data source
- Replace the null values by proper values based on data dict type [ numerical or category ]
- Convert the category values in Ordinal cols to be the scale discreate values

### 2. EDA and Feature Engineering
- Encode the category cols by using OneHotEncoder
- normalization by using StandardScaler

### 3. Get pre-predictos from correlation between features and target 
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


**Evaluation and Conceptual Understanding**
- Does the student accurately identify and explain the baseline score?
- Does the student select and use metrics relevant to the problem objective?
- Is more than one metric utilized in order to better assess performance?
- Does the student interpret the results of their model for purposes of inference?
- Is domain knowledge demonstrated when interpreting results?
- Does the student provide appropriate interpretation with regards to descriptive and inferential statistics?

**Conclusion and Recommendations**
- Does the student provide appropriate context to connect individual steps back to the overall project?
- Is it clear how the final recommendations were reached?
- Are the conclusions/recommendations clearly stated?
- Does the conclusion answer the original problem statement?
- Does the student address how findings of this research can be applied for the benefit of stakeholders?
- Are future steps to move the project forward identified?


### Conclusion

	States policy make a significant change in participation rate. 
	All students must check States policy before taking a Test.

