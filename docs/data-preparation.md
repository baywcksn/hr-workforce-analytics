# Data Preparation — HR Workforce Analytics

## 1. Overview

This stage prepares the IBM HR Analytics Employee Attrition dataset for further analysis using SQL and Power BI.

The preparation process focuses on maintaining data integrity, identifying unnecessary columns, and creating an analysis-ready dataset.

## 2. Source Dataset

| Attribute | Description |
|---|---|
| Dataset | IBM HR Analytics Employee Attrition & Performance |
| Source Records | 1,470 employees |
| Original Columns | 35 |
| Prepared Columns | 32 |
| File Format | CSV |

## 3. Data Quality Assessment

The following checks were performed:

| Assessment | Result |
|---|---|
| Missing Values | 0 found across all 35 columns |
| Duplicate EmployeeNumber | 0 found |
| Duplicate Records | No row reduction observed during the check |
| Invalid Values | No anomalies identified in the validation performed |
| Constant Columns | 3 identified |

## 4. Data Preparation Activities

Three constant columns were removed from the analysis dataset:

| Column | Constant Value | Reason |
|---|---|---|
| EmployeeCount | 1 | No variation across employees |
| Over18 | Y | No variation across employees |
| StandardHours | 80 | No variation across employees |

The original dataset was preserved in the `Raw Data` worksheet.

A separate worksheet named `Analysis Data` was created for analytical preparation.

## 5. Final Dataset

| Attribute | Value |
|---|---:|
| Total Employees | 1,470 |
| Total Columns | 32 |
| Total Rows Including Header | 1,471 |

## 6. Tools Used

- Microsoft Excel
- Excel Filter
- Excel COUNTBLANK
- Excel COUNTIF
- Excel Remove Duplicates

## 7. Next Stage

The prepared dataset will be used for SQL-based analysis, focusing on employee attrition, workforce demographics, compensation, job satisfaction, and work experience.