# TSA-Claims-Data-Analysis
This project is a data analysis and cleaning task involving TSA (Transportation Security Administration) claims data from 2002 to 2017. The objective of the project is to import, clean, and analyze the data to extract meaningful insights.
Here’s a breakdown of the project's key steps:

1) Library Setup and Data Import:

A SAS library is created to store the data.
TSA claims data is imported from a CSV file into a SAS dataset.

2) Data Preview and Structure Analysis:

The first 20 rows of the imported dataset are printed to preview the data.
The structure of the dataset is analyzed using the PROC CONTENTS procedure.

3) Data Cleaning:

Missing values and placeholder values like "-" are replaced with "Unknown".
Inconsistent values in the Claim_Type and Disposition columns are standardized.
Duplicate rows are removed.
The dataset is sorted by Incident_Date.

4) Column Cleaning and Formatting:

Specific columns (Claim_Site, Disposition, Claim_Type) are cleaned and standardized.
State codes are converted to uppercase, and state names are formatted to proper case.

5) Date Validation:

A new column (Date_Issues) is created to flag records with date inconsistencies (e.g., dates outside the 2002-2017 range, missing dates, or Incident_Date later than Date_Received).

6) Labeling and Formatting:

Permanent labels and formats are added to columns for better readability.
Unnecessary columns (County and City) are dropped from the dataset.

7) Report Generation:

An overall report is generated in PDF format.
Frequency analysis is performed to identify the distribution of date issues.
Yearly distribution of claims is visualized.
Specific analysis for California is performed, including:
Frequencies of claim types, claim sites, and dispositions.
Statistics (mean, min, max, sum) for Close_Amount.
