# Factors-Influencing-Airbnb-Pricing-in-Barcelona-A-Predictive-Analysis-Using-Linear-Regression
### Note: This project is organized into multiple branches on GitHub, each correlating with a different portion of the assignment. To explore specific sections, please select the branch that corresponds to the task or analysis you are interested in. 

This project analyzes the Barcelona Airbnb listings dataset to identify key factors influencing pricing in the city's short-term rental market. It explores property attributes like location, amenities, and host characteristics, using linear regression to quantify the relationship between these factors and nightly prices.

# Branches: 
## *>Branch 1: Data Import, Initial Exploration, Cleaning, and Preprocessing<*
### •	1.1. Reading a CSV File into R
### •	1.2. Checking Missing and Empty Values in the Data Frame
### •	1.3. Cleaning and Transforming the Dataset
### •	1.4  Data Cleaning and Imputation for Missing Values
### •	1.5 Final Data Cleaning and Validation

## *>Branch 2: Feature Engineering, Model Development and Feature Selection<*
### •	2.1. Feature Engineering and Encoding for Property Listings Dataset
### •	2.2. Linear Model Development with All Attributes and Feature Selection for Price Prediction
### •	2.3. Multicollinearity Assessment and Attribute Refinement
### •	2.4. Stepwise Regression and Post-Refinement of Attributes

## *>Branch 3: Model Refinement and Outlier Detection<*
### •	3.1. Linear Model After Stepwise Regression
### •	3.2. Residual Plot Before Removal of Outliers
### •	3.3. Removing Outliers and Visualizing Residuals
### •	3.4. Linear Model with Significant Attributes After Outlier Removal

## *>Branch 4: Final Model Development and Evaluation<*
### •	4.1. Final Removal of Outliers and Fitting the Final Linear Model
### •	4.2. Final Model Evaluation and Multicollinearity Check
### •	4.3. Random Forest Model Development and Evaluation

## *>Branch 5: Model Summary and Final Reporting<*
### •	5.1. Results Summary
### •	5.2. Insights and Next Steps

# Assignment Outcome: Comparison of Models
The below section presents a comparison of two types of regression models—**Linear Regression** and **Random Forest**—evaluated through various iterations. Below is a detailed summary of the model performances, showing improvements from the initial models to the final versions.

---

## 1. **First Linear Regression Model**:
   - **Residual Standard Error**: 341  
   - **R-squared**: 37.41%  
   - **Adjusted R-squared**: 35.33%  
   - **F-statistic**: 17.98  
   - **p-value**: < 2.2e-16

   The first linear regression model had a low R-squared, indicating poor predictive power. The large residual error suggested the model was not a good fit for the data.

---

## 2. **First Random Forest Model**:
   - **Mean Squared Residuals**: 32,789.3  
   - **Explained Variance**: 81.76%

   The first random forest model showed a good improvement over the linear regression model, explaining 81.76% of the variance. However, there was still room for improvement in terms of prediction accuracy.

---

## 3. **Last Linear Regression Model**:
   - **Residual Standard Error**: 33.57  
   - **R-squared**: 92.7%  
   - **Adjusted R-squared**: 92.68%  
   - **F-statistic**: 3394  
   - **p-value**: < 2.2e-16

   The last linear regression model significantly improved, explaining 92.7% of the variance. The smaller residual error demonstrated better prediction accuracy.

---

## 4. **Last Random Forest Model**:
   - **Mean Squared Residuals**: 1004.815  
   - **Explained Variance**: 93.47%

   The final random forest model showed exceptional predictive power, explaining 93.47% of the variance with a drastically reduced mean squared residual. This was the most accurate model in terms of predictive performance.

---

## **Conclusion**:

- **Overall Comparison**:  
   Both the **final linear regression** and **random forest models** showed substantial improvements over the initial versions. The **random forest model** outperformed the linear regression models, with both the last random forest and linear regression models achieving nearly identical explained variance (around 93%).

- **Best Performing Model**:  
   The **last random forest model** was the most robust, achieving the highest accuracy and lowest residual error, making it the top performer.

---

## **Model Results Summary Table**:

| Model                    | Residual Standard Error | R-squared | Explained Variance | Mean Squared Residuals |
|--------------------------|-------------------------|-----------|---------------------|------------------------|
| Initial Linear Regression     | 341                     | 37.41%    | N/A                 | N/A                    |
| Initial Random Forest         | N/A                     | N/A       | 81.76%              | 32,789.3               |
| Final Linear Regression    | 33.57                   | 92.7%     | N/A                 | N/A                    |
| Final Random Forest        | N/A                     | N/A       | 93.47%              | 1004.815               |

---
