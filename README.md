# Branch 3: Model Refinement and Residual Analysis
## •	3.1. Third Linear Model Development and Analysis After Stepwise Regression
- Fitted a refined linear model (third model) using predictors selected after the stepwise regression process.

![results - third](https://github.com/user-attachments/assets/4750853b-7169-46ec-b76a-3977a526e488)
![regression values - third](https://github.com/user-attachments/assets/8fe5012d-ca8d-471b-a535-5a1503c2ba1a)


## •	3.2. Residual Plot Before Handling Large Residuals
- Visualized the residuals to assess any patterns or unusually large residuals that might affect model accuracy.

![residualplotthird](https://github.com/user-attachments/assets/d0cff96a-1ad9-46c9-bfd8-5c16dc1d0d55)


## •	3.3. Identifying and Removing Data Points with Large Residuals
- Detected and removed observations where the residuals fell outside the acceptable range, as defined by the interquartile range (IQR) thresholds.
- Data points with residuals outside the range Q1 – 1.5 * IQR, Q3 + 1.5 * IQR were treated as "outliers" in terms of model fit. These points were removed to refine the model.

![3 3](https://github.com/user-attachments/assets/a4c95dd4-ec1a-4928-8e0b-a9fc83fcb619)


## •	3.4. Fourth Linear Model Development with Significant Attributes After Handling Large Residuals
- Refitted the linear model after removing data points with large residuals and assessing its performance.

![results - fourth](https://github.com/user-attachments/assets/52034091-4b4d-4597-99a6-3e4a664e8c99)
![residuals values - fourth](https://github.com/user-attachments/assets/43d91a95-4d73-433a-b03f-4b3952217ba7)


## •	3.5. Residual Plot After Handling Large Residuals
- Reassessed residual distribution to ensure randomness and absence of discernible patterns.

![residualplotfourth](https://github.com/user-attachments/assets/caae0eec-eb20-4111-9747-6c29d09955a8)
