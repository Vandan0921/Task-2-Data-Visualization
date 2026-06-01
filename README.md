# Power BI Data Import and Transformation Project

## Project Overview

This project demonstrates how to import, clean, transform, and integrate data from multiple sources in Power BI Desktop. The project uses VanArsdel sales data from Microsoft Learning and covers data preparation techniques including filtering, appending, unpivoting, and data transformation.

---

## Tools Used

* Power BI Desktop
* Microsoft Access Database
* CSV Files
* Microsoft Excel

---

# Exercise 1: Import Data from Access Database

## Objective

Import sales-related data from an Access database and perform initial transformations before loading the data model.

## Imported Tables

* bi_date
* bi_geo
* bi_manufacturer
* bi_product
* bi_salesFact

## Transformations Performed

### bi_salesFact

* Changed Date column data type to Date.
* Filtered records to include dates after December 31, 1999.

### bi_date

* Changed Date column data type to Date.
* Filtered records to include dates after December 31, 1999.

### Query Renaming

| Original Table  | Renamed Query |
| --------------- | ------------- |
| bi_date         | Date          |
| bi_geo          | Locations     |
| bi_manufacturer | Manufacturers |
| bi_product      | Products      |
| bi_salesFact    | Sales         |

## Result

Data was successfully loaded into Power BI Desktop and validated in Data View.

---

# Exercise 2: Import Data from Folder Containing CSV Files

## Objective

Import international sales data from multiple CSV files and combine it with existing US sales data.

## Data Source

Folder containing four CSV files with international sales records.

## Transformations Performed

### International Sales Query

* Combined all CSV files into a single query.
* Renamed query to International Sales.
* Filtered records after December 31, 1999.
* Removed Source.Name column.

### Sales Query

* Appended International Sales data to the existing Sales table.
* Added custom column:

Country Name =

* Country value if available

* "USA" if Country is null

* Removed Country column.

## Result

US and International sales data were consolidated into a single Sales table.

---

# Exercise 3: Import Less Structured Data from Excel

## Objective

Import and reshape population data from an Excel report.

## Data Source

Country Population Excel file.

## Transformations Performed

* Renamed query to Country Population.
* Removed first four rows.
* Promoted first row to headers.
* Unpivoted yearly columns into rows.
* Renamed columns:

  * Attribute → Year
  * Value → Population
* Removed Year 1999 records.
* Changed data types:

  * Year → Whole Number
  * Population → Whole Number

## Result

Population data was transformed into an analysis-ready format suitable for data modeling and reporting.

---

# Key Power BI Features Used

* Get Data
* Query Editor
* Data Type Transformation
* Row Filtering
* Append Queries
* Custom Columns
* Remove Columns
* Promote Headers
* Unpivot Columns
* Data Modeling

---

# Learning Outcomes

By completing this project, I learned how to:

* Import data from multiple sources.
* Transform and clean datasets.
* Combine datasets using Append Queries.
* Create custom calculated columns.
* Reshape unstructured data using Unpivot.
* Prepare data for reporting and visualization in Power BI.

---

# Repository Contents

* README.md
* Screenshots
* Dataset References

---
**[Live Report 1](https://app.powerbi.com/view?r=eyJrIjoiNTI1Yjg2Y2QtZTBlMi00NjhlLThlMjMtODZhM2YyMzNkOTJhIiwidCI6Ijc1ZGYwOTZjLThiNzItNDhlNC05YjkxLWNiZjc5ZDg3ZWUzYSIsImMiOjl9)**

## Author

Vandan

Power BI Data Preparation and Transformation Project
