# Employee Attendance & Workforce Analytics Dashboard

## Overview

This project is an enterprise-level **Employee Attendance Analytics Dashboard** developed using **Microsoft Power BI** to monitor workforce attendance behavior, employee punctuality, work hours, absenteeism, and department-level attendance trends.

The solution provides HR teams and management with actionable insights into:

* Late arrivals
* Early leaves
* Absenteeism trends
* Employee work hours
* Department attendance performance
* Holiday utilization
* Workforce productivity metrics

The dashboard was designed to improve operational visibility, reduce manual HR reporting, and support data-driven workforce management decisions.

---

# Dashboard Screenshots

## Attendance Overview Dashboard

<img width="1326" height="736" alt="Attendance overview" src="https://github.com/user-attachments/assets/f3150ac8-5359-4336-947c-a25a2c77137a" />


---

## Late Arrival Analytics Dashboard

 <img width="1338" height="728" alt="Late Arrivals" src="https://github.com/user-attachments/assets/96108dbc-f44a-4c28-a196-ab789fac0dae" />


---

# Business Problem

The organization lacked a centralized reporting system for monitoring employee attendance behavior across departments. HR teams relied heavily on manual Excel reports, making it difficult to:

* Identify attendance trends
* Monitor late arrivals and early leaves
* Track employee work hours
* Compare department attendance performance
* Generate management-level reports efficiently

---

# Solution

Developed an interactive Power BI solution integrating attendance datasets to provide:

* Real-time attendance analytics
* Department-wise attendance tracking
* Employee-level late arrival monitoring
* Work-hour analysis
* KPI-based HR reporting
* Drill-down and filtering capabilities

The dashboard enables HR and leadership teams to identify workforce patterns and improve attendance management processes.

---

# Key Features

## Attendance KPIs

* Average Check-In Time
* Average Check-Out Time
* Total Absents
* Total Sick Leaves
* Holidays Taken
* Remaining Holidays
* Alternate Off Days

---

## Attendance Trend Analysis

* Late Arrival Trends by Year
* Early Leave Trends
* Work Hours Comparison
* Department Performance Monitoring

---

## Department Analytics

* Late Arrival Counts by Department
* Attendance Comparison Across Teams
* Employee Attendance Distribution

---

## Employee-Level Insights

* Individual attendance analysis
* Late arrival counts by employee
* Drill-through reporting
* Attendance pattern tracking

---

# Technologies Used

| Technology                      | Purpose                      |
| ------------------------------- | ---------------------------- |
| Microsoft Power BI              | Dashboard Development        |
| Power Query                     | Data Transformation          |
| DAX                             | KPI Calculations & Measures  |
| SQL                             | Data Extraction & Querying   |
| Data Modeling                   | Relationship & Schema Design |
| Excel / Attendance Data Sources | Source Data                  |

---

# Power BI Features Implemented

* Interactive Dashboards
* Drill-through Navigation
* KPI Cards
* Custom DAX Measures
* Department-Level Filtering
* Data Modeling
* Trend Analysis
* Employee Attendance Analytics
* Dynamic Visualizations
* Slicers & Cross Filtering

---

# Sample DAX Measures

## Late Arrival Count

```DAX
Late Arrival Count =
CALCULATE(
    COUNT(Attendance[EmployeeID]),
    Attendance[LateArrival] = "Yes"
)
```

---

## Average Check-In Time

```DAX
Average Check In =
FORMAT(
    AVERAGE(Attendance[CheckInTime]),
    "hh:mm:ss"
)
```

---

# Data Model Architecture

```text
Attendance Source Files / SQL Database
                ↓
          Power Query ETL
                ↓
        Data Cleaning & Modeling
                ↓
          DAX Calculations
                ↓
         Power BI Data Model
                ↓
      Interactive Dashboards
                ↓
      HR & Management Insights
```

---

# Business Impact

* Improved workforce attendance visibility
* Reduced manual HR reporting effort
* Enabled department-level attendance monitoring
* Helped identify recurring late attendance patterns
* Improved decision-making for HR operations

---

# Future Enhancements

* Power BI Service Deployment
* Row-Level Security (RLS)
* Automated Data Refresh
* Email Alert Integration
* Mobile Dashboard Optimization
* Predictive Attendance Analytics

---

# Author

### Power BI Developer | Data Analytics Engineer

Specialized in:

* Power BI
* DAX
* Data Modeling
* SQL
* ETL
* Power Platform
* Business Intelligence Solutions
