# Datat Cleaning and Preparation

## Overview:

The Adidas sales dataset was cleaned and prepared primalry using SQL, however certain data quality issues such as formatting inconsistencies and a small number of missing values—were more efficiently resolved in Excel.

## Handling Missing Values

•	The City column contained 13 missing values and the State column contained 10 missing values.

•	These values were manually reviewed and corrected using contextual information to ensure data accuracy.

## Sales Method Missing Value:

•	The SalesMethod column had 11 missing values.

•	Due to insufficient information to accurately determine the correct category, missing values were replaced with “Unknown” to preserve data integrity.

## Operating Margin Calculation

•	The OperatingMargin column contained 5 missing values.

•	These values were calculated using the formula:
Operating Margin = Operating Profit ÷ Total Sales

## Data Format Corrections

A small number of records in the InvoiceDate column were incorrectly formatted (MM/DD/YYYY instead of DD/MM/YYYY).
These were manually corrected due to the limited number of affected rows, ensuring consistency in date formatting.

## Data Validation (Total Sales Issue)

•	It was identified that the TotalSales column was incorrectly calculated in the original dataset.
The correct formula is:
Total Sales = Price Per Unit × Units Sold

•	The dataset contained values that were 10 times higher than expected.
This issue was corrected by recalculating Total Sales using the correct formula.

