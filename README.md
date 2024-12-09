# Branch 1: Data Import, Initial Exploration, Cleaning, and Preprocessing
### > FILE: 
    - Credit Score - Prediction, Scoring and Implementation.sas
    - New_Data.csv
    - scored_new_data_creditscore.csv

## •	1.1. Importing and Previewing the Dataset
- Importing the CSV File: Loaded the data from the specified file path.
- Previewing the Dataset: Displayed the first few rows of the dataset using head().

## •	1.2. Checking for Missing and Empty Values
- Identifying Empty Values: Detected columns with empty string values using sapply().
- Identifying Missing Values: Detected missing values (NA) in each column.
- Dataset Structure: Viewed the structure of the dataset using str().

## •	1.3. Cleaning and Transforming the Dataset
- Removing Irrelevant Columns: Dropped unnecessary attributes to streamline the dataset.
- Binary Encoding: Converted specific text attributes (e.g., neighborhood_overview, space, access) into binary indicators (1 for presence, 0 for absence).
- Cleaning Numeric Columns:
  - Convertedcleaning_fee from text to numeric by removing dollar signs and spaces.
  - Replaced missing or empty values in cleaning_fee with the column's median.   

## •	1.4  Data Cleaning and Imputation for Missing Values
- Imputation with Medians: Replaced missing values (NA) in numeric columns (e.g., bathrooms, bedrooms, beds, review_scores) with the column median.
- Imputation for square_feet:
  - Replaced NA or zero values with the neighborhood average.
  - For neighborhoods lacking valid square_feet data, used the grouped average by neighbourhood_group_cleansed.
## •	1.5 Final Data Cleaning and Validation
- Final Type Conversion: Ensured price and cleaning_fee are numeric by rechecking conversions.
-	Validation:
    - Confirmed there are no remaining missing values (NA) or empty strings.
    - Performed a final structural review of the cleaned dataset using str().


