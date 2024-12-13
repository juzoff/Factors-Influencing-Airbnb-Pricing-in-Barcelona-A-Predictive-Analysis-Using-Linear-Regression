# Branch 5: Final Model Evaluation & Comparison: Predictions on Training vs. Test Sets, Analysis, and Performance Metrics for First vs. Final Linear Models

### > FILE: 
    - Barcelona Airbnb listings - Linear Modeling.Rmd


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

![5 3a](https://github.com/user-attachments/assets/a30691f0-b8c3-4238-8852-822311ba712e)
<img src="https://github.com/user-attachments/assets/c1577093-c43c-43eb-ac4d-575e1307f2ac" width="600" />

- The final model significantly outperforms the first model in all metrics. While the first model has low R-squared values (37.6% for training, 34.2% for testing) and high errors (RMSE ~336 for training, ~342 for testing), the final model achieves much higher R-squared values (93.1% for training, 91.5% for testing) and drastically lower errors (RMSE ~33.5 for both sets). The improvement reflects better accuracy, reduced prediction errors, and strong generalization, due to better feature selection, model tuning, or addressing issues such as overfitting or outliers.

<img src="https://github.com/user-attachments/assets/bc8c99d0-54e4-4f96-9309-0da850915311" width="600" />
<img src="https://github.com/user-attachments/assets/df5a4cc1-0d2f-4a42-95f7-a114b2d49e6a" width="600" />

- These two scatter plots show Actual vs. Predicted Price from a linear model, and they illustrate improvements between an initial and a final model.
   - Key Observations:
      1.	First Model:
         - The predictions are widely scattered around the diagonal "perfect prediction" line (dashed).
        	- There are many points far from the line, indicating poor predictions and a lack of fit.
         - Extreme variability is visible, especially for higher actual prices (e.g., beyond 2000 on the x-axis), where predictions deviate significantly.
      2. Final Model:
         - The points are tightly clustered around the diagonal line, showing much better alignment between predicted and actual values.
         - The variance in predictions has reduced significantly, indicating a stronger and more accurate fit.
         - The model performs well across all price ranges without extreme deviations.
   - Overall Difference:
      - The final model is much more accurate and consistent compared to the first. It suggests significant improvements, likely through better feature selection, hyperparameter tuning, or cleaning of data.
      - The first model is poor at generalizing, while the final model aligns well with the actual data.

<img src="https://github.com/user-attachments/assets/9c70fe0f-bba8-4e1c-afd1-0c5f9a433f57" width="600" />

- The two histograms compare the distribution of residuals (errors) from two linear models: the First Linear Model on the left and the Final Linear Model on the right.
  - First Linear Model (Left):
    - The residuals are highly concentrated around 0 but have an extremely narrow range with only a few very large outliers visible on both sides.
    - This indicates that the model likely has issues, such as poor handling of the data's variability or outliers dominating the residual distribution.
  - Final Linear Model (Left):
    - The residuals are more evenly distributed and form a bell-shaped curve centered around 0.
    - This suggests that the model fits the data better, with a more normal distribution of residuals and fewer extreme outliers.
- Key Difference:
  - The first model has a poorly distributed set of residuals with extreme outliers, while the final model achieves a more balanced and well-behaved residual distribution, improving the fit.




