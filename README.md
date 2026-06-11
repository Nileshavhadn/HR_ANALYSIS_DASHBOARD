# 📊 HR Analysis Dashboard

## Overview

The HR Analysis Dashboard is an interactive Power BI project designed to analyze workforce demographics, employee attrition, job satisfaction, performance ratings, and education-based trends. The dashboard helps HR professionals and business leaders make data-driven decisions to improve employee retention and organizational performance.

---

## Dashboard Preview

<img width="1495" height="830" alt="HR_ANALYSIS_DASHBOARD" src="https://github.com/user-attachments/assets/6df12a9b-3b12-4ffa-8468-1a5d8cf6e0ba" />




## Features

### Employee Overview
- Total workforce count
- Active employees
- Average employee age
- Overall attrition statistics

### Department-wise Attrition
Analyze employee turnover across:
- Research & Development (R&D)
- Sales
- Human Resources (HR)

### Education Field Analysis
Attrition trends by educational background:
- Medical
- Life Sciences
- Technical Degree
- Marketing
- Other

### Job Satisfaction Analysis
Measure satisfaction levels across job roles:
- Sales Executive
- Sales Representative
- Research Scientist
- Research Director
- Manufacturing Director

### Performance Rating Distribution
Visual representation of employee performance ratings.

### Attrition by Gender & Age Group
Demographic analysis of attrition across:
- Under 25
- 25–34
- 35–44
- 45–54
- Over 55

### Interactive Filters
Education-level slicer:
- Associate Degree
- Bachelor's Degree
- Master's Degree
- Doctoral Degree
- High School

---

## Business Questions Answered

- Which department has the highest attrition?
- Which education field experiences the most employee turnover?
- How does job satisfaction vary by role?
- Which age groups are most likely to leave?
- What is the current attrition rate?
- How does employee performance relate to attrition?

---

## Tools & Technologies

- Power BI Desktop
- Power Query
- DAX (Data Analysis Expressions)
- Data Modeling
- Data Visualization

---

## DAX Measures

### Attrition Count

```DAX
Attrition Count =
CALCULATE(
    COUNT(Employee[EmployeeID]),
    Employee[Attrition] = "Yes"
)
```

### Attrition Rate

```DAX
Attrition Rate =
DIVIDE(
    [Attrition Count],
    [Total Employees]
)
```

### Active Employees

```DAX
Active Employees =
[Total Employees] - [Attrition Count]
```

### Average Age

```DAX
Average Age =
AVERAGE(Employee[Age])
```

---

## Insights

- Overall attrition rate is approximately **18%**.
- Sales and R&D departments contribute the largest share of employee turnover.
- Medical and Life Sciences educational backgrounds show higher attrition counts.
- Most employees have a performance rating of **3**.
- Attrition patterns differ significantly across age groups and genders.

---



## Future Enhancements

- Predictive Attrition Analytics
- Employee Tenure Analysis
- Salary & Compensation Dashboard
- Recruitment Analytics
- Diversity & Inclusion Metrics
- Employee Engagement Tracking
