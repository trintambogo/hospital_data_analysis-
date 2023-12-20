# Hospital Data Analysis

## Overview

The hospital data analysis involved exploring a dataset with 15,757 rows and 56 columns, focusing on missing values, correlations, data cleaning, and visualization. Here's a summary of the key steps and findings:

## Data Overview

- **Number of Rows and Columns:**
  - The dataset comprised 15,757 rows and 56 columns.

- **Missing Values:**
  - Eight columns had missing values.

## Data Cleaning

1. **Handling Non-Numeric Values:**
   - Converted non-numeric values to NaN in columns with missing values.

2. **Converting Columns to Numeric:**
   - Converted columns with missing values to numeric.

3. **Correlation Analysis:**
   - Explored column correlations using a heatmap to inform data cleaning strategies.

4. **Handling Missing Values:**
   - **BNP Column:**
     - Dropped due to high missing values (>50%).

   - **EF Column:**
     - Replaced missing values with the mode (60) based on moderate correlation with prior CMD.

   - **Glucose and TLC Columns:**
     - Used forward fill due to close values.

   - **Platelets and Glucose Columns:**
     - Used backward fill due to close values.

   - **HB Column:**
     - Filled missing values using the median based on a strong correlation with anaemia.

   - **Creatinine Column:**
     - Filled missing values based on CKD column grouping.

   - **Urea Column:**
     - High correlation between urea and creatinine. 
     - Filled missing values based on creatinine grouping. 
   - **Chest Infection Column:**
     - Converted invalid inputs to NaN and used forward fill.

5. **Checking for Duplicates:**
   - No duplicates were found.

6. **Feature Engineering:**
   - Engineered arrival and discharge date columns.

## Visualization

1. **Commonly Admitted Diseases:**
   - CAD, HTM, ACS, DM, and heart failure were the most common diseases with 4000 and above cases.

2. **Monthly Admissions Trend (2017-2019):**
   - Observed fluctuations in monthly admissions in 2019.
   - A sudden rise in number of admissions from March to April 2017.
   - January had the highest number of admissions in 2019.
   - admissions from April to December 2019 were roughly constant. 
   - highest number of admissions of the years from July to November 2018 

3. **Leading Causes of Deaths:**
   - Heart failure, AKI, ACS, and SHOCK had the highest number of deaths, with men leading across diseases.

4. **Trend in Deaths Over the Years:**
   - Noticed a rise in deaths from 2017 to 2018 and a subsequent decrease in 2019.

5. **Disease Distribution Across Age Groups:**
   - CAD affected people aged 61-80, HTN and heart failure affected those aged 81 and above, and ACS affected individuals aged 41-60.

6. **Admissions Across Urban and Rural Areas:**
   - Most admissions were from people in urban areas over the years.

## Conclusion

The analysis provided insights into disease patterns, admission trends, causes of deaths, and demographics in the hospital dataset. It serves as a comprehensive overview of the dataset, its cleaning process, and key findings.
