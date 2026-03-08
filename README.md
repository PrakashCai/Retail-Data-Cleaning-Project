Project Overview

This project focuses on cleaning and preparing a "dirty" retail dataset originally sourced from [Kaggle]

(Link:- https://www.kaggle.com/datasets/ahmedmohamed2003/retail-store-sales-dirty-for-data-cleaning/data). 

The goal was to transform messy, real-world data into a structured format suitable for analysis using Excel Power Query. 

Input = dirty_retail_store_sales.csv (Original)

Output = clean_retail_store_sales.xlsx (Final Output)


License: This project uses data from Kaggle, licensed under [Insert License Name, e.g., CC BY-SA 4.0].


Tools Used :- Power Query in Microsoft Power BI : Used for data transformation and cleaning. 


Actions :- 

Handling Missing Values: Identified nulls in the columns by first looking for anchor column. 

Imputed the item names from corresponding Category column.

Data Type Conversion: Standardized the Data type of Columns.

Text Standardization: Used TRIM and CLEAN functions to remove extra spaces and non-printable characters from product names.

Removing Duplicates: Checked for duplicate records. (Not found)

Conditional Columns: Created a new columns price per qty based on total spent and quantity. Imputed missing quantity as a '1' because 
the payment method tell that cash was received for that transaction, so that i got total spent values also.

'Key insight' = In the first attempt I directly removed the missing values of 'item' column (as they were only 5%) and due to removing them other columns missing values are also got deleted. After that continued the cleaning and EDA. In the 2nd attempt decided to impute missing values from
corresponding Category column as there was relation between Category and item name. So by not removing missing values I have not missed the 
valuable information of that transaction. 

Final Result :- The dataset was successfully cleaned and structured, making it ready for analysis, reporting, and visualization tasks.
N/A Handling :-  Discount column has True, False and N/A values. Replaced N/A value by 'False' as generally in retail there is True only
if discount is given.
