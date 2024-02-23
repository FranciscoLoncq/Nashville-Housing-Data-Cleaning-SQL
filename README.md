# Nashville Housing Data Exploration - SQL
## Overview:
This project showcases data cleaning on a dataset containing home value data in the thriving Nashville market using SQL. The primary goal is to enhance data quality, making it more suitable for analysis and reporting.

## Transformations Applied:
### Data Cleaning and Standardization:
Standardized date formats by converting SaleDate from DateTime to Date.
Populated missing PropertyAddress values using a self-join on ParcelID.
### Structural Data Transformations:
Broke down the PropertyAddress into individual columns (Address and City).
Split OwnerAddress into separate columns for Address, City, and State.
### Data Type Conversion:
Converted the binary representation of SoldAsVacant to a more readable format (YES or NO).
Altered column types to accommodate changes in data representation.
### Data Quality Improvement:
Handled duplicate rows using a Common Table Expression (CTE) and ROW_NUMBER() to identify and keep only unique rows.
###  SQL Query Optimization:
Ordered and filtered data as needed for analysis and review.
## Main Results:
### Missing Property Addresses:
Identified and populated missing PropertyAddress values by leveraging information from other rows with the same ParcelID.
### Address and City Separation:
Successfully split PropertyAddress into Address and City columns for better data organization.
### Owner Address Parsing:
Extracted individual components (Address, City, State) from the OwnerAddress column.
###  SoldAsVacant Representation Improvement:
Transformed binary values in the SoldAsVacant column into a more understandable 'YES' or 'NO' format.
### Duplicate Removal:
Detected and removed 104 duplicate rows based on specific columns, improving data integrity.
### Unused Columns Deletion:
Removed unnecessary columns (OwnerAddress, TaxDistrict, PropertyAddress) to streamline the dataset.

These applied transformations and findings collectively contribute to the project's success in enhancing data quality for subsequent analysis and reporting purposes.

## Links:
### Nashville Housing Dataset (CSV)
[Dataset: Nashville Housing Data for Data Cleaning](https://github.com/FranciscoLoncq/Nashville-Housing-Data-Exploration-SQL/blob/main/Nashville%20Housing%20Data%20for%20Data%20Cleaning.csv)

### SQL Query
[Data Cleaning Query](https://github.com/FranciscoLoncq/Nashville-Housing-Data-Exploration-SQL/blob/main/SQL_Data_Cleaning_Project_NashvilleHousing.sql)

### Credits
Alex Freberg

