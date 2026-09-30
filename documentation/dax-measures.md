# DAX Measures


```DAX
Total Employees =
COUNTROWS('WA_Fn-UseC_-HR-Employee-Attrition')

Attrition Count =
CALCULATE(
    COUNTROWS('WA_Fn-UseC_-HR-Employee-Attrition'),
    'WA_Fn-UseC_-HR-Employee-Attrition'[Attrition] = "Yes"
)

Attrition Rate =
DIVIDE(
    [Attrition Count],
    [Total Employees],
    0
)

Average Monthly Income =
AVERAGE(
    'WA_Fn-UseC_-HR-Employee-Attrition'[MonthlyIncome]
)

Average Job Satisfaction =
AVERAGE(
    'WA_Fn-UseC_-HR-Employee-Attrition'[JobSatisfaction]
)

Average Work-Life Balance =
AVERAGE(
    'WA_Fn-UseC_-HR-Employee-Attrition'[WorkLifeBalance]
)

Average Environment Satisfaction =
AVERAGE(
    'WA_Fn-UseC_-HR-Employee-Attrition'[EnvironmentSatisfaction]
)

