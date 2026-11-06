# Business Questions & KPI

## 1. Business Questions

The following business questions will guide the HR Workforce Analytics analysis.

| No. | Business Question | Analysis Focus |
|:---:|---|---|
| 1 | How many employees have left the company? | Attrition Count |
| 2 | What is the overall employee attrition rate? | Attrition Rate |
| 3 | Which department has the highest attrition rate? | Department Analysis |
| 4 | Which age group has the highest attrition rate? | Age Group Analysis |
| 5 | How does monthly income differ between employees who left and those who stayed? | Compensation Analysis |
| 6 | How does job satisfaction relate to employee attrition? | Satisfaction Analysis |

## 2. Key Performance Indicators (KPIs)

| KPI | Definition | Calculation |
|---|---|---|
| Total Employees | Total number of employees. | COUNT(EmployeeNumber) |
| Attrition Count | Number of employees who left. | COUNT where Attrition = 'Yes' |
| Active Employees | Number of employees who remain. | Total Employees − Attrition Count |
| Attrition Rate | Percentage of employees who left. | (Attrition Count / Total Employees) × 100% |
| Average Monthly Income | Average monthly employee income. | AVG(MonthlyIncome) |
| Average Job Satisfaction | Average job satisfaction score. | AVG(JobSatisfaction) |

## Notes

- Dataset contains 1,470 employee records.
- Attrition values are categorized as `Yes` and `No`.
- Attrition rate is calculated against the total number of employees.
- The analysis identifies patterns and associations, not causation.