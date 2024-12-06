# Branch 2: Feature Engineering, Encoding for Property Listings Dataset, and First Random Forest Model
## •	2.1. Feature Engineering, Encoding for Property Listings Dataset, and First Random Forest Model
- Engineering New Features: The amenities and host_verifications columns were originally in a list format, requiring preprocessing and tokenization. This involved cleaning the data by removing unnecessary characters and splitting the list values into distinct tokens for better analysis.
- Created Binary Indicator Variables: Generated binary columns for each unique amenity and host verification, representing the presence of these features in each listing.
- Categorical Encoding: Encoded categorical variables into dummy variables for further modeling using caret::dummyVars().
- Developed an initial Random Forest model as a baseline for comparison with subsequent models, providing a benchmark to evaluate the effectiveness of feature engineering and feature selection techniques.
![randomforestfirst](https://github.com/user-attachments/assets/ff2c1f3f-be8b-46e4-8809-9ea1fa24cb2c)
![randomforestfirstvi](https://github.com/user-attachments/assets/0cc4bc46-fa9c-4f0e-933f-391b73d15a75)


## •	2.2. First Linear Model Development and Feature Selection for Price Prediction
- First Linear Model: Fitted an initial linear regression model using all features to predict price as a baseline for comparison with subsequent models.

![results - initial](https://github.com/user-attachments/assets/9a034494-f891-42d2-a9de-0a92b12e8094)
![regression values - initial](https://github.com/user-attachments/assets/dd3d9a11-2dab-4a52-98c8-3819f9d34ad6)

- Creating Residual Plot from First Linear Model.

![residualplot](https://github.com/user-attachments/assets/5d68181e-f06f-474a-88fe-2deba2b11de7)
  
- Feature Significance: Identifed significant predictors (with p-values < 0.10) based on the model's summary, and created a new model with only these significant features.

## •	2.3. Multicollinearity Assessment and Attribute Refinement
- Variance Inflation Factor (VIF) Calculation: Evaluated multicollinearity in the dataset by calculating VIF for each feature in the model.
- Removing Highly Collinear Features: Identified features with VIF > 10 and removed them to avoid multicollinearity, ensuring more stable model results.

## •	2.4  Stepwise Regression and Post-Refinement of Attributes
- Stepwise Regression: Applied stepwise regression (stepAIC) to further refine the model by selecting the most relevant features, while removing redundant predictors.
- Post-Stepwise Attribute Refinement: After stepwise regression, removed any additional irrelevant or redundant attributes identified during the process.
- Model Evaluation: Validated the model's performance and check for any remaining issues such as high multicollinearity or insignificant predictors.




