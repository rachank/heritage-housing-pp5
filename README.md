# Heritage Housing 

## Project Overview
- Client: Lydia Doe inherited 4 houses in Ames, Iowa, USA. She is from Belgium and has no knowledge of the local property markets. Therefore there is a risk of undervaluing or overvaluing the properties without further local information.
- This project creates a web dashboard using ML to predict the local house prices for Ames, Iowa
- The Live App: Will be deployed on Heroku upon project completion
- Repository: https://github.com/rachank/heritage-housing-pp5.git


## Dataset Summary
- Source: [Code Institute on Kaggle](https://www.kaggle.com/codeinstitute/housing-prices-data)
- From Ames, Iowa, USA, informaiton on 1,460 house sale records
- Each record contains 23 features covering physical house attributes
- The target variable: SalePrice in USD
- Features include:
    - Size: GrLivArea, TotalBsmtSF, 1stFlrSF 
    - Quality: OverallQual, OverallCond (rated 1-10)
    - Age: YearBuilt, YearRemodAdd
    - Garage: GarageCars, GarageArea
    - Rooms: FullBath, TotRmsAbvGrd, BedroomAbvGr


## Business Requirements
- 2 requirements outlined:

**1 - Correlation Study**
- The clients wants to know the house attributes that correlate with the sale price
- Requires data visualisations of correlated variables against the sale price

**2 - Price Prediction**
- The client requires predicted sale prices for her 4 houses in Ames, Iowa
- The client wants to predict the price for any house in Ames, Iowa


**User Stories**

- As the client I want to understand what drives the property value in the area of Ames, Iowa, through the correlation of sale price and features.
- As the client I want to predict the sale price of 4 inherited houses in order to make informed selling decisions.
- As the client I want to predict the price of any house in Ames, Iowa, in order to have a valuation tool for the future.


**Project Epics (CRISP-DM)**

- Information gathering and collection of data
- Data visualisation, cleaning and preparation
- Model training, opimisation and validation
- Dashboard planning, dsigning and development
- Dashboard deployment and release


## Hypothesis and Validation

**Hypothesis 1**

- Claim: Higher overall quality rating will lead to a higher sale price
- Validation: Pearson correlation study of OverallQual vs SalePrice
- Conclusion: To be confirmed following the completion of the correlation study

**Hypothesis 2**

- Claim: Above ground living area is a top 3 predictor of price
- Validation: Pearson and Spearman correction of GrLivArea
- Conclusion: To be confirmed following the completion of the correlation study


**Hypothesis **

- Claim: Newer houses sell for more than older houses do
- Validation: Scatter plot 
- Conclusion: To be confirmed following the completion of the correlation study


## Rationale

**BR1 maps to:**
- Conventional data analysis - no ML needed for this requirement
- Pearson and Spearman correlation study on full dataset
- Heatmap of correleations between key variables and SalePrice
- Scatter plots of top correlated features vs SalePrice
- Written interpretation accompanying every visualisation 

**BR2 maps to:**
- the supervised machine learning regression tasks
- Scikit-learn pipeline: data cleaning to feature engineering
to scaling to regressor model to predicted price in USD
- Pipeline embedded in dashboard for real time predictions
- .filter method applied to live data to ensure correct feature order and prevent silent prediction errors


