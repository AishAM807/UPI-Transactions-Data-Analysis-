# UPI Transactions Data Analysis 

### Dashboard Link :


### Data Source : Excel 


## Problem Statement:

With the rapid adoption of Unified Payments Interface (UPI) in India, digital transactions have grown exponentially across individuals, merchants, and financial institutions. However, the increasing volume of transactions generates large datasets that are often underutilized for deriving meaningful insights.

This project aims to analyze UPI transaction data to understand user behavior, transaction trends, payment success rates, and peak usage patterns. The objective is to identify key performance indicators such as transaction volume, transaction value distribution, failure rates, and top contributing merchant categories.



### Steps followed

- Step 1: Load data into Power BI Desktop, dataset is a excel workbook file.
- Step 2: Open power query editor & in view tab under Data preview section, check "column distribution", "column quality" & "column profile" options.
- Step 3: Also since by default, profile will be opened only for 1000 rows so you need to select "column profiling based on entire dataset".
- Step 4: Validated the data types across all columns and updated them to ensure accurate and consistent data formatting.
- Step 5: On the report page, added 10 slicers and arranged them appropriately using horizontal and vertical alignment to enhance dashboard usability and visual consistency.
- Step 6: Created a calculated column using DAX to classify customers into distinct age groups according to their age.

		Age Group = IF('UPI Transaction'[CustomerAge] <= 25, "A1",
			    IF( 'UPI Transaction'[CustomerAge] <=35 ,"A2", "A3"))

- Step 7: Assigned relevant data fields to the 10 slicers.
- Step 8: To maintain consistency and accommodate all required slicers, Report Page 2 was created by duplicating Report Page 1, preserving the existing layout and visual structure.
