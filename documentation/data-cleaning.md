# Data Cleaning & Transformation

## Tool

Power Query in Power BI Desktop.

## Data Quality Checks

The dataset was reviewed using:

- Column Quality
- Column Distribution
- Column Profile

The dataset was checked for blank values, errors, and data consistency.

## Duplicate Validation

Employee records were checked using `EmployeeNumber`.

No duplicate employee records were identified.

## Removed Columns

The following redundant fields were removed:

- EmployeeCount
- EmployeeNumber
- Over18
- StandardHours

## Derived Columns

### Age Group

Employees were grouped into:

- 18–25
- 26–35
- 36–45
- 46–55
- 56+

So that we can work on data easily

### Salary Band

Monthly income was grouped into:

- Low
- Lower-Mid
- Mid
- Upper-Mid
- High

### Tenure Band

Years at company was grouped into:

- New
- Early Career
- Established
- Experienced
- Long Tenure

## Data Types

Numeric fields and categorical fields were validated and assigned
appropriate data types for analysis.
