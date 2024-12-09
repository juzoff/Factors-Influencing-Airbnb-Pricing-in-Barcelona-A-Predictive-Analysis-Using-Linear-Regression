# Branch 5: Final Model Evaluation & Comparison: Predictions on Training vs. Test Sets, Analysis, and Performance Metrics for First vs. Final Linear Models
## •	5.1. First Linear Model: Prediction Analysis, Actual vs Predicted Comparison, and Residuals
- Generated Predictions: The predict() function was used with the trained first linear model to generate predictions on the dataset.
- Compared Actual vs Predicted: A data frame was created combining the actual values and their corresponding predicted values to facilitate comparison.
- Calculated Residuals: Residuals were calculated by subtracting predicted values from actual values, and these were added as a new column to the comparison data frame for analysis.
   - Top 5 - Largest Residuals: The top five largest residuals indicate significant discrepancies between actual and predicted values, highlighting areas where the first linear model struggles. The residuals are extremely high, ranging from approximately 7,049 to 8,812, suggesting that the model is consistently underpredicting for these instances. These results are expected, as this was the initial linear model developed without refinement, likely lacking important predictor adjustments or interactions. The weak results and high residuals underscore the need for further model optimization.

![5 1](https://github.com/user-attachments/assets/1eb8b2a9-94f4-43dd-bb9d-747c154eb801) 

## •	5.2. Final Linear Model: Prediction Analysis, Actual vs Predicted Comparison, and Residuals
- Generated Predictions: The predict() function was used with the trained final linear model to generate predictions on the dataset.
- Compared Actual vs Predicted: A data frame was created combining the actual values and their corresponding predicted values to facilitate comparison.
- Calculated Residuals: Residuals were calculated by subtracting predicted values from actual values, and these were added as a new column to the comparison data frame for analysis.
- Top 5 - Largest Residuals: The top five residuals from the final model demonstrate a marked improvement in performance compared to the first model. Residuals are significantly smaller, ranging from approximately 144 to 182, indicating much closer alignment between actual and predicted values. This reflects the model's ability to capture key predictors and interactions effectively. The strong performance of the final model highlights the benefits of refinement and optimization, showcasing its robustness and accuracy in predictions compared to the initial model with much larger residuals.


![5 2](https://github.com/user-attachments/assets/2fde14b5-685d-46c7-99b2-44a06860f335)


## •	5.3. Model Training, Testing, Performance Metrics, and Visualization Analysis	
- Split Data and Train Models: The dataset was split into training (70%) and testing (30%) sets using random sampling. Two linear models were trained: the first and final linear models. These models were built using all available predictors.
- Evaluate Model Performance: Predictions were made on the testing sets. Performance metrics such as Mean Squared Error (MSE), Root Mean Squared Error (RMSE), and R-squared (R²) values were calculated for both training and testing sets for both the first and final models.
- Visualization of Results: Visualizations were created to analyze the models' performance. Scatter plots compare actual vs predicted values, and histograms show the distribution of residuals for both models to examine prediction errors and residual patterns.

