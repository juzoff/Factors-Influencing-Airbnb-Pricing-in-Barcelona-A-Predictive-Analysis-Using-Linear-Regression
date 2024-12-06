# Branch 3: Feature Engineering, Encoding for Property Listings Dataset, and First Random Forest Model
## •	3.1. Linear Model Analysis After Stepwise Regression
- Fitting a refined linear model using predictors selected after the stepwise regression process.

## •	3.2. Residual Plot Before Handling Large Residuals
- Visualizing the residuals to assess any patterns or unusually large residuals that might affect model accuracy.

## •	3.3. Identifying and Removing Data Points with Large Residuals
- Detecting and removing observations where the residuals fall outside the acceptable range, as defined by the interquartile range (IQR) thresholds.
- Data points with residuals outside the range Q1 – 1.5 * IQR, Q3 + 1.5 * IQR are treated as "outliers" in terms of model fit. These points are removed to refine the model.

## •	3.4. Linear Model with Significant Attributes After Handling Large Residuals
- Refitting the linear model after removing data points with large residuals and assessing its performance.

## •	3.5. Residual Plot After Handling Large Residuals
- Reassessing residual distribution to ensure randomness and absence of discernible patterns.
