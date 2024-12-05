# Branch 1: Data Import, Initial Exploration, Cleaning, and Preprocessing
## •	1.1. Importing and Previewing the Dataset
### - Importing the CSV File: Load the data from the specified file path.
### - Previewing the Dataset: Display the first few rows of the dataset using head().
## •	1.2. Checking for Missing and Empty Values
### - Identifying Empty Values: Detect columns with empty string values using sapply().
### - Identifying Missing Values: Detect missing values (NA) in each column.
### - Dataset Structure: View the structure of the dataset using str().
## •	1.3. Cleaning and Transforming the Dataset
### - Removing Irrelevant Columns: Drop unnecessary attributes to streamline the dataset.
### - Binary Encoding: Convert specific text attributes (e.g., neighborhood_overview, space, access) into binary indicators (1 for presence, 0 for absence).
### - Cleaning Numeric Columns:
#### >Convert cleaning_fee from text to numeric by removing dollar signs and spaces.
#### >Replace missing or empty values in cleaning_fee with the column's median.   
## •	1.4  Data Cleaning and Imputation for Missing Values
### - Imputation with Medians: Replace missing values (NA) in numeric columns (e.g., bathrooms, bedrooms, beds, review_scores) with the column median.
### - Imputation for square_feet:
#### >Replace NA or zero values with the neighborhood average.
#### >For neighborhoods lacking valid square_feet data, use the grouped average by neighbourhood_group_cleansed.
## •	1.5 Final Data Cleaning and Validation
### - Final Type Conversion: Ensure price and cleaning_fee are numeric by rechecking conversions.
### -	Validation:
#### >Confirm there are no remaining missing values (NA) or empty strings.
#### >Perform a final structural review of the cleaned dataset using str().


