# 🔹 Project 1: Attendance Data Analysis System (Excel)

## 📌 Project Overview

This project focuses on analyzing student attendance data using
Microsoft Excel. The objective was to clean raw data, calculate
attendance metrics, and generate summary reports with visual insights.

------------------------------------------------------------------------

## 🗂 Dataset Structure

  Student_ID   Student_Name   Class   Date         Status
  ------------ -------------- ------- ------------ ---------
  101          Rahul          IT-A    01-01-2026   Present
  102          Sneha          IT-A    01-01-2026   Absent

------------------------------------------------------------------------

## 🧹 Step 1: Data Cleaning

-   Removed duplicate records
-   Handled missing values
-   Standardized "Present/Absent" entries
-   Used Filters and Sorting for organization

------------------------------------------------------------------------

## 📊 Step 2: Attendance Calculations

### ✅ Total Present Days

``` excel
=COUNTIFS(Raw_Data!A:A,101,Raw_Data!E:E,"Present")
```

### ✅ Total Absent Days

``` excel
=COUNTIFS(Raw_Data!A:A,101,Raw_Data!E:E,"Absent")
```

### ✅ Total Working Days

``` excel
=COUNTIF(Raw_Data!A:A,101)
```

### ✅ Attendance Percentage

``` excel
= (Present_Days / Total_Working_Days) * 100
```

------------------------------------------------------------------------

## 📈 Step 3: Pivot Table & Visualization

-   Created Pivot Table (Rows: Student_Name, Columns: Status)
-   Used Count of Status
-   Generated Column Chart for trend analysis

------------------------------------------------------------------------

## 🎯 Skills Demonstrated

-   Data Cleaning\
-   Excel Formulas (COUNTIF, COUNTIFS)\
-   Pivot Tables\
-   Data Visualization\
-   Reporting & Insights

------------------------------------------------------------------------


