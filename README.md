# Branch 2: Feature Engineering, Model Development, and Feature Selection
## •	2.1. Feature Engineering and Encoding for Property Listings Dataset
- Engineering New Features: The amenities and host_verifications columns were originally in a list format, requiring preprocessing and tokenization. This involved cleaning the data by removing unnecessary characters and splitting the list values into distinct tokens for better analysis.
- Created Binary Indicator Variables: Generated binary columns for each unique amenity and host verification, representing the presence of these features in each listing.
- Categorical Encoding: Encoded categorical variables into dummy variables for further modeling using caret::dummyVars().

## •	2.2. Initial Linear Model Development and Feature Selection for Price Prediction
- Initial Linear Model: Fitted an initial linear regression model using all features to predict price.
- Feature Significance: Identifed significant predictors (with p-values < 0.10) based on the model's summary, and created a new model with only these significant features.

**PUT HERE RESIDUAL PLOT AND RESULTS OF INITIAL linear model**

## •	2.3. Multicollinearity Assessment and Attribute Refinement
- Variance Inflation Factor (VIF) Calculation: Evaluated multicollinearity in the dataset by calculating VIF for each feature in the model.
- Removing Highly Collinear Features: Identified features with VIF > 10 and removed them to avoid multicollinearity, ensuring more stable model results.

## •	2.4  Stepwise Regression and Post-Refinement of Attributes
- Stepwise Regression: Applied stepwise regression (stepAIC) to further refine the model by selecting the most relevant features, while removing redundant predictors.
- Post-Stepwise Attribute Refinement: After stepwise regression, removed any additional irrelevant or redundant attributes identified during the process.
- Model Evaluation: Validated the model's performance and check for any remaining issues such as high multicollinearity or insignificant predictors.




