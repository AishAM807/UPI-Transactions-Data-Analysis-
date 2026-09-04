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
- Step 9: Added a line chart on the first report page to display monthly transaction amounts and identify transaction trends over time. Also, added a Currency filter in the filter pane to enable analysis of transaction amounts by selected currency.
- Step 10: Enhanced the second report page with a matrix visual that provides a comprehensive breakdown of Total Amount and Remaining Balance by Transaction Month, City, and Currency, enabling detailed analysis of transaction performance across multiple dimensions.
- Step 11: Implemented the Sync Slicers feature to synchronize all filters between Page 1 and Page 2, allowing users to apply consistent filtering across both report pages.


<img width="420" height="264" alt="Image" src="https://github.com/user-attachments/assets/cd3a82f4-605b-441c-8e30-92e577614dc2" />


- Step 12: Applied conditional formatting to the matrix visual to highlight price variations using background colors based on the lowest and highest price values.

  
<img width="938" height="655" alt="Image" src="https://github.com/user-attachments/assets/cde13fdc-a669-4073-8fb4-1a059b5eca21" />


  
- Step 13: Implemented Power BI bookmarks by duplicating the existing line chart and converting the duplicate into a column chart. Configured the Selection Pane and Bookmarks Pane to control visual visibility and enable interactive navigation between the two chart views.
  

<img width="962" height="449" alt="Image" src="https://github.com/user-attachments/assets/49d8e180-a7fc-41b6-bdac-2deee213a505" />

<img width="973" height="551" alt="Image" src="https://github.com/user-attachments/assets/c0a92745-36d4-4ade-89a7-a0201bcf5e7d" />

<img width="432" height="545" alt="Image" src="https://github.com/user-attachments/assets/cbf1de1c-9546-4955-93c0-aa791326a5d7" />


- Step 14: Published the completed Power BI report to Power BI Service for online access and interactive data analysis.


 
 # Report Snapshot (Power BI DESKTOP)

<img width="871" height="486" alt="Image" src="https://github.com/user-attachments/assets/3383cbe5-5d22-40b7-9338-01c26cbaa484" />


<img width="881" height="493" alt="Image" src="https://github.com/user-attachments/assets/76ac82ee-ed05-4117-afc0-4e3f5cd187dd" />
