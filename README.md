# Branch 4: Final Model Development and Evaluation
## •	4.1. Selection of Significant Attributes for Fifth Linear Model
- Fitted a fifth linear regression model on the cleaned dataset from 3.4 (after removing large residuals).
- Extracted predictors with p-values below the 0.08 threshold, excluding the intercept.
- Constructed a new formula and refitted the model with these significant attributes.

![results - fifth](https://github.com/user-attachments/assets/96253a5f-524e-4be9-bd06-b1df78d7479b)
![residual - fifth](https://github.com/user-attachments/assets/46075474-9516-41c4-bc01-17d43fbd3c38)


## •	4.2. Final Linear Model Development After Handling Large Residuals
- Detected and removed observations in the fifth linear model where the residuals fell outside the acceptable range, as defined by the interquartile range (IQR) thresholds.

![residual removal](https://github.com/user-attachments/assets/c9dde6b0-e482-4747-9ff6-aa08d9d70151)

  
- Data points with residuals outside the range Q1 – 1.5 * IQR, Q3 + 1.5 * IQR were treated as "outliers" in terms of model fit. These points were removed to refine the model.
- A final linear regression model was developed using the refined dataset, ensuring improved model accuracy and robustness after addressing large residuals.

![results final](https://github.com/user-attachments/assets/5d13f4a7-c89c-482e-bb4d-ae05ec5177e1)
![residuals final](https://github.com/user-attachments/assets/5fb8c4d2-5e02-4296-8690-fabfd50c5b40)

## •	4.3. Final Linear Model Evaluation and Multicollinearity Check
- Performed residual analysis by plotting residuals versus fitted values to ensure randomness.
- Conducted a final multicollinearity check using Variance Inflation Factor (VIF) to ensure that there no potential collinearity issues.

![residuallm - final](https://github.com/user-attachments/assets/652b61f3-31ac-43a7-b48e-620f64677911)

## •	4.4. Final Random Forest Model Development
- Performed residual analysis by plotting residuals versus fitted values to ensure randomness.
- Conducted a final multicollinearity check using Variance Inflation Factor (VIF) to ensure that there no potential collinearity issues.

