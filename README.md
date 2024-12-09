# Factors-Influencing-Airbnb-Pricing-in-Barcelona-A-Predictive-Analysis-Using-Linear-Regression
### Note: This project is organized into multiple branches on GitHub, each correlating with a different portion of the assignment. To explore specific sections, please select the branch that corresponds to the task or analysis you are interested in. 

This project delves into the Barcelona Airbnb listings dataset to uncover key insights into the factors that influence pricing in the city’s short-term rental market. By analyzing a wide range of property attributes such as location, amenities, and host characteristics, the project aims to identify the primary drivers behind Airbnb pricing in Barcelona. The analysis employs linear regression as the core predictive model to quantify the relationship between these variables and the price per night. Additionally, a thorough data cleaning process was carried out, including the removal of large residuals to ensure the integrity of the results.

​The goal of the project was not only to build an accurate pricing model but also to understand which features have the most significant impact on pricing decisions, thereby providing actionable insights for hosts and industry stakeholders. In the process, advanced techniques such as variable selection based on statistical significance, multicollinearity checks, and stepwise regression. These steps helped refine the model and ensure its reliability. By leveraging both linear regression and other machine learning models like Random Forest, the project highlights the effectiveness of predictive analytics in understanding complex pricing dynamics within the Airbnb pricing economy.

# Assignment Outcome: Comparison of Models
The below section presents a comparison of two types of regression models—**Linear Regression** and **Random Forest**—evaluated through various iterations. Below is a detailed summary of the model performances, showing improvements from the first models to the final versions.

---

## 1. **First Linear Regression Model**:
   - **Residual Standard Error**: 341  
   - **R-squared**: 37.41%  
   - **Adjusted R-squared**: 35.33%  
   - **F-statistic**: 17.98  
   - **p-value**: < 2.2e-16

   The first linear regression model had a low R-squared, indicating poor predictive power. The large residual error suggested the model was not a good fit for the data.

![results - initial](https://github.com/user-attachments/assets/9a034494-f891-42d2-a9de-0a92b12e8094)
![regression values - initial](https://github.com/user-attachments/assets/dd3d9a11-2dab-4a52-98c8-3819f9d34ad6)

![residualplot](https://github.com/user-attachments/assets/5d68181e-f06f-474a-88fe-2deba2b11de7)

---

## 2. **First Random Forest Model**:
   - **Mean Squared Residuals**: 31,264.6  
   - **Explained Variance**: 82.61%

   The first random forest model showed a good improvement over the linear regression model, explaining 81.76% of the variance. However, there was still room for improvement in terms of prediction accuracy.

![randomforestfirst](https://github.com/user-attachments/assets/38e7f4d8-af2d-4750-9061-6d6ff634060f)
![randomforestfirstvi](https://github.com/user-attachments/assets/0cc4bc46-fa9c-4f0e-933f-391b73d15a75)
![residualrf](https://github.com/user-attachments/assets/1dcd2cd6-87c0-4a14-a28f-ecef402928e7)


---

## 3. **Final Linear Regression Model**:
   - **Residual Standard Error**: 33.57  
   - **R-squared**: 92.7%  
   - **Adjusted R-squared**: 92.68%  
   - **F-statistic**: 3394  
   - **p-value**: < 2.2e-16

   The final linear regression model significantly improved, explaining 92.7% of the variance. The smaller residual error demonstrated better prediction accuracy.

![results final](https://github.com/user-attachments/assets/d92868d3-72ca-4235-bafd-94e994f71158)
![residuals final](https://github.com/user-attachments/assets/8c7027c9-4064-41d5-be48-f4cde432884b)

![residuallm - final](https://github.com/user-attachments/assets/284f11e2-a5bc-44d1-921e-00b8cc7a20d2)


---

## 4. **Final Random Forest Model**:
   - **Mean Squared Residuals**: 1004.815  
   - **Explained Variance**: 93.47%

   The final random forest model showed exceptional predictive power, explaining 93.47% of the variance with a drastically reduced mean squared residual. This was the most accurate model in terms of predictive performance.

![randomforestfinal](https://github.com/user-attachments/assets/ff22dc11-f5f4-40d5-8f68-25498ec6d94e)
![randomforestfinalvi](https://github.com/user-attachments/assets/7ac8eefd-9af1-4f7c-94cb-ee335f22ae45)
![randomforestfinalrp](https://github.com/user-attachments/assets/63614139-3865-4011-8c67-829ee6703f67)


---

## **Conclusion**:

- **Overall Comparison**:  
   Both the **final linear regression** and **random forest models** showed substantial improvements over the initial versions. The **random forest model** outperformed the linear regression models, with both the last random forest and linear regression models achieving nearly identical explained variance (around 93%).

- **Best Performing Model**:  
   The **last random forest model** was the most robust, achieving the highest accuracy and lowest residual error, making it the top performer.

---

## **Model Results Summary Table**:


| Model                    | Residual Standard Error | R-squared | Explained Variance | Mean Squared Residuals | Results                                           | Residual Plot                                   |
|--------------------------|-------------------------|-----------|---------------------|------------------------|-------------------------------------------------|------------------------------------------------|
| First Linear Regression  | 341                     | 37.41%    | N/A                 | N/A                    | ![results - initial](https://github.com/user-attachments/assets/9a034494-f891-42d2-a9de-0a92b12e8094)   | ![residualplot](https://github.com/user-attachments/assets/5d68181e-f06f-474a-88fe-2deba2b11de7) |
| First Random Forest      | N/A                     | N/A       | 82.61%              | 31264.6                | ![randomforestfirst](https://github.com/user-attachments/assets/38e7f4d8-af2d-4750-9061-6d6ff634060f)   | ![residualrf](https://github.com/user-attachments/assets/1dcd2cd6-87c0-4a14-a28f-ecef402928e7) |
| Final Linear Regression  | 33.57                   | 92.7%     | N/A                 | N/A                    | ![results final](https://github.com/user-attachments/assets/d92868d3-72ca-4235-bafd-94e994f71158)   | ![residuallm - final](https://github.com/user-attachments/assets/284f11e2-a5bc-44d1-921e-00b8cc7a20d2) |
| Final Random Forest      | N/A                     | N/A       | 93.47%              | 1004.815               | ![randomforestfinal](https://github.com/user-attachments/assets/ff22dc11-f5f4-40d5-8f68-25498ec6d94e)  | ![randomforestfinalrp](https://github.com/user-attachments/assets/63614139-3865-4011-8c67-829ee6703f67)                                            |

---

# Branches: 
## *>Branch 1: Data Import, Initial Exploration, Cleaning, and Preprocessing<*
### •	1.1. Importing and Previewing the Dataset
### •	1.2. Checking for Missing and Empty Values
### •	1.3. Cleaning and Transforming the Dataset
### •	1.4  Data Cleaning and Imputation for Missing Values
### •	1.5 Final Data Cleaning and Validation

## *>Branch 2: Feature Engineering, Model Development and Feature Selection<*
### •	2.1. Feature Engineering, Encoding for Property Listings Dataset, and First Random Forest Model
### •	2.2. First Linear Model Development, Feature Selection for Price Prediction, and Second Linear Model Development
### •	2.3. Multicollinearity Assessment and Attribute Refinement
### •	2.4. Stepwise Regression and Post-Refinement of Attributes

## *>Branch 3: Model Refinement and Residual Analysis<*
### •	3.1. Third Linear Model Development and Analysis After Stepwise Regression
### •	3.2. Residual Plot Before Handling Large Residuals
### •	3.3. Identifying and Removing Data Points with Large Residuals
### •	3.4. Fourth Linear Model Development with Significant Attributes After Handling Large Residuals
### •	3.5. Residual Plot After Handling Large Residuals


## *>Branch 4: Final Model Development and Evaluation<*
### •	4.1. Selection of Significant Attributes for Fifth Linear Model
### •	4.2. Final Linear Model Development After Handling Large Residuals
### •	4.3. Final Linear Model Residual Analysis/Evaluation and Multicollinearity Check
### •	4.4. Final Random Forest Model Development
### •	4.5. Final Random Forest Residual Analysis/Evaluation

## *>Branch 5: Final Model Evaluation & Comparison: Predictions on Training vs. Test Sets, Analysis, and Performance Metrics for First vs. Final Linear Models<*
### •	5.1. First Linear Model: Prediction Analysis, Actual vs Predicted Comparison, and Residuals
### •	5.2. Final Linear Model: Prediction Analysis, Actual vs Predicted Comparison, and Residuals
### •	5.3. Model Training, Testing, Performance Metrics, and Visualization Analysis

