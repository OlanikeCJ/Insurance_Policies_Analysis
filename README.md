# Car Insurance Policies Analysis
![dashboard](https://github.com/OlanikeCJ/Insurance_Policies_Analysis/blob/main/Images%20%20-%20insurance/dashboard.png?raw=true)

## Project Description

This project analyzes car insurance policies and claims to identify patterns in customer behavior, claim frequency, and financial impact. The insights can help other businesses optimize risk assessment, pricing strategies, and policy offerings.

## Dataset Structure

The dataset contains customer and car insurance details, with the following key columns:

![datset](https://github.com/OlanikeCJ/Insurance_Policies_Analysis/blob/main/Images%20%20-%20insurance/dataset.png?raw=true)

## Dataset Cleaning Process (ETL)

The dataset was processed and cleaned using the following steps:

> Extracted the CSV file into Power BI.

> Changed data types in Power Query for accurate analysis.

> Merged the car_make and car_model columns for clarity.

> Created an age column by calculating the customer's age from the birthdate.

> Added an age category column to group customers into different age brackets.

Snapshot of cleaned data:
![cleaned_data](https://github.com/OlanikeCJ/Insurance_Policies_Analysis/blob/main/Images%20%20-%20insurance/cleaned%20dataset.png?raw=true)


## Calculations

I created the following DAX measures to enable analysis and answer key business questions:

``` DAX
Avg Claim Frequency = AVERAGE('Insurance Policies'[claim_freq])
Avg Insurance Claim Amount = AVERAGE('Insurance Policies'[claim_amt])
Total Car Makes = DISTINCTCOUNT('Insurance Policies'[car_make_and_model])
Total Claim Frequency = SUM('Insurance Policies'[claim_freq])
Total Customers = DISTINCTCOUNT('Insurance Policies'[ID])
Total Household Income = SUM('Insurance Policies'[household_income])
```

## Conclusion: 

### Business Questions Answered

The analysis was structured around the following business questions:

 > *1. What is the distribution of car usage based on gender and the presence of kids driving?*

 > *2. Which car makes and models are most frequently involved in insurance claims, and what is the average claim amount for each?*

 > *3. Is there a correlation between education level and claim frequency or claim amount?*

 > *4. How does car color correlate with claim frequency and claim amount?*

 > *5. What is the average claim amount across different coverage zones?*

 > *6. How does household income relate to claim frequency and claim amount?*
  
         
  To answer these questions, the following insights were generated:

> Classified total customers by gender to understand the gender distribution.

> Analyzed kids driving by car use and gender to identify patterns in shared vehicle usage.

> Calculated the average insurance claim amount by car use and model to determine the most expensive claims.

> Measured total claim frequency by educational level to explore potential correlations between education and claim behavior.

> Calculated the average insurance claim amount by coverage zone to assess regional risk levels.

> Created slicers for car color and car make/model to allow for interactive data filtering.

See the dashboard snapshot for detailed visual insights and data trends.

