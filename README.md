# Branch 7: Machine Learning Pipeline

### > FILE: 
    - Barcelona Airbnb listings - Linear Modeling.Rmd

## •	Pipeline #1 - Data Preparation and Model Training
- Data Preparation: It organizes and cleans the raw Airbnb listings data, ensuring that it is in a usable format for analysis. This includes removing irrelevant information, converting textual data into numerical or binary formats, and handling missing values effectively.
- Feature Engineering: The pipeline generates meaningful features from the data, such as binary indicators for amenities and host verifications, which can enhance the predictive power of the model. This step is crucial for capturing the complexities of rental characteristics that may influence pricing.
- Model Training and Evaluation: It builds a linear regression model to predict rental prices based on the processed dataset. By splitting the data into training and testing sets, the pipeline allows the evaluation of the model's performance using metrics like Mean Absolute Error (MAE) and Root Mean Squared Error (RMSE). This helps in understanding how well the model can generalize to new, unseen data.


## •	Pipeline #2 - New Dataset
- Data Loading and Cleaning: The pipeline begins by loading a new dataset of Airbnb listings, followed by the removal of irrelevant attributes and the cleaning of specific variables like "cleaning_fee" and "price" to ensure they are in a usable numerical format.
- Imputation and Feature Engineering: Missing values are imputed using median values for selected features. The pipeline also preprocesses features related to amenities and host verifications by creating binary indicators and one-hot encoding categorical variables.
- Model Integration and Predictions: After preparing the data, the pipeline loads a pre-trained linear regression model and checks for any missing attributes necessary for predictions. If any are missing, they are imputed using regression to ensure compatibility with the model, and predictions for rental prices are generated and added back to the dataset.
- Results Compilation: Finally, the pipeline compiles the predicted prices into a new dataframe while optionally merging these predictions with the original dataset, and displays the results for review.
