# FTW3-Day5
### Housing Prices Regression

#### Data Treatment 
- used nyc-rolling-sales.csv
- converted SALE PRICE, LAND SQUARE FEET, GROSS SQUARE FEET to float
- coverted SALE DATE to datetime64, but only used the the year for the features
- removed zero sale prices, then the 5% and 95% outliers
- dummy variables for NEIGHBORHOOD, BUILDING CLASS AT TIME OF SALE, TAX CLASS AT PRESENT, BUILDING CLASS AT PRESENT
- used numeric features: 'GROSS SQUARE FEET','LAND SQUARE FEET','LOT','BOROUGH','BLOCK','LOT','ZIP CODE','RESIDENTIAL UNITS','COMMERCIAL UNITS','TOTAL UNITS','YEAR BUILT','TAX CLASS AT TIME OF SALE','YEAR'
- outcome variable: SALE PRICE
- filled null featueres -- fillna(0)

## Linear Regression
RMSE = 511459.2792821024

## Decision Tree
RMSE = 584072.64556654

## KNeighbors
RMSE = 527054.0135616323

## Random Forest
RMSE = _not enough memory_

## Elastic Net
RMSE = 608031.9767543538
_CovergenceWarning: Objective did not converge._

## Ridge
RMSE = 510729.6975818353

## Lasso
RMSE = 511064.6153937624
_CovergenceWarning: Objective did not converge._

## Artificial Neural Network
RMSE = _not enough memory_

### Recommendations
- clean the features (drop outliers)
- study other parameters of each model for the models to be tweaked

