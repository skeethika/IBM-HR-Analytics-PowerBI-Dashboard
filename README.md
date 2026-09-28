# IBM-HR-Analytics-PowerBI-Dashboard
Interactive IBM HR Analytics dashboard developed using Power BI to analyse employee attrition, workforce demographics, compensation, and employee satisfaction.
# IBM HR Analytics – Power BI Dashboard

## Project Overview

This project presents an interactive **IBM HR Analytics Dashboard** developed using **Microsoft Power BI**. The dashboard analyses employee workforce data to understand **employee attrition, compensation, satisfaction, and workforce demographics**.

The project demonstrates the use of **Power Query, DAX, data visualization, and interactive dashboard design** for Human Resource Analytics.

## Objectives

* Analyse overall employee workforce
* Identify employee attrition patterns
* Analyse attrition by department and job role
* Examine the relationship between overtime and attrition
* Analyse employee compensation
* Study employee satisfaction
* Analyse workforce demographics
* Create an interactive HR analytics dashboard

##  Tools & Technologies

* Microsoft Power BI
* Power Query
* DAX
* CSV Dataset
* Data Visualization

## Dataset

The project uses the **IBM HR Analytics Employee Attrition & Performance dataset**.
-<a href="https://www.kaggle.com/datasets/pavansubhasht/ibm-hr-analytics-attrition-dataset?utm_source=chatgpt.com">
-<a href="https://github.com/skeethika/IBM-HR-Analytics-PowerBI-Dashboard/edit/main/README.md">

The dataset contains employee information including:

* Age
* Gender
* Department
* Job Role
* Job Level
* Monthly Income
* Overtime
* Job Satisfaction
* Environment Satisfaction
* Performance Rating
* Total Working Years
* Years at Company
* Attrition

## Dashboard Pages

### 1. HR Workforce Overview

Provides an overall view of the workforce using KPI cards and charts.

**Key metrics:**

* Total Employees
* Attrition Count
* Attrition Rate
* Average Monthly Income
* Average Age
<img width="415" height="239" alt="Screenshot 2026-09-28 195458" src="https://github.com/user-attachments/assets/1b972bda-b4dc-47f6-9329-3334d68e401c" />


### 2. Attrition Analysis

Analyses employee attrition across different workforce categories.

**Key analysis:**

* Attrition by Department
* Attrition by Job Role
* Attrition by Overtime
* Attrition by Job Satisfaction

### 3. Compensation Analysis

Analyses employee income and compensation patterns.

**Key analysis:**

* Average Income by Department
* Average Income by Job Role
* Average Income by Job Level
* Income vs Years at Company

### 4. Employee Satisfaction

Analyses different employee satisfaction dimensions.

**Key analysis:**

* Job Satisfaction
* Environment Satisfaction
* Relationship Satisfaction
* Work-Life Balance
* Job Involvement

### 5. Workforce Demographics

Provides an overview of employee demographic characteristics.

**Key analysis:**

* Gender
* Age
* Education
* Marital Status
* Department
* Job Level

## 📐 Key DAX Measures

```DAX
Total Employees = COUNTROWS(HR_Data)
```

```DAX
Attrition Count =
CALCULATE(
    COUNTROWS(HR_Data),
    HR_Data[Attrition] = "Yes"
)
```

```DAX
Attrition Rate =
DIVIDE(
    [Attrition Count],
    [Total Employees],
    0
)
```

```DAX
Average Monthly Income =
AVERAGE(HR_Data[MonthlyIncome])
```

```DAX
Average Age =
AVERAGE(HR_Data[Age])
```

##  Key Features

* Interactive KPI cards
* Department and job-role analysis
* Attrition analysis
* Compensation analysis
* Employee satisfaction analysis
* Workforce demographic analysis
* Interactive slicers
* DAX-based HR metrics
* Interactive Power BI visualizations

##  Business Value

The dashboard transforms raw employee data into meaningful visual insights that can support HR analysis and workforce planning. It provides an interactive way to explore employee attrition, compensation, satisfaction, and demographic patterns.

##  Project Outcome

This project demonstrates practical skills in:

* Power BI
* Power Query
* DAX
* Data Cleaning
* Data Visualization
* Business Analytics
* HR Analytics
* Dashboard Development

## Author

**Keerthika S.**

MBA – HR & Business Analytics

## Disclaimer

This project is created for **academic and learning purposes** using the publicly available IBM HR Analytics dataset.
