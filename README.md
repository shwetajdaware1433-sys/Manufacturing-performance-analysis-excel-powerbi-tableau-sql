# Manufacturing-performance-analysis-excel-powerbi-tableau-sql

## Table of Contents
- [Projet Overview](#project-overview)
- [Objective](#objective)
- [Project Components](project_conponents)
- [Technical Steps Followed](#technical-steps-followed)
- [Dashboard Features](#dashboard-features)
- [Repository Structure](#repository-structure)
- [Key Insights](#key-insights)
- [Tools used](#tools-used)
- [Challenges and Solutions](#challenges-and-solutions)
- [Future Enhancements](#future-enhancements)
- [Conclusion](#conclusion)
  
### Project Overview

This project focuses on analyzing end-to-end manufacturing performance using multiple BI and analytics tools. The goal is to identify production efficiency, rejected quantities, wastage levels, employee/machine performance, and departmental manufacturing trends using interactive dashboards and data-driven insights.
The analysis was performed using:
 - Excel for data cleaning, preparation, pivot tables, and basic visualization
 - SQL for querying raw manufacturing data, aggregating KPIs, and building analytical    datasets
 - Power BI for detailed dashboards and DAX-based calculations
 - Tableau for dynamic visual exploration and trend-based insights


### Objective

- Understand overall production output and rejection reasons
- Compare manufactured vs rejected quantities
- Identify employees and machines contributing to the highest rejections
- Track department-wise production trends
- Support management in decision-making to reduce wastage and optimize production    flow

### Project Components

1. Excel
   - Data cleaning (removing nulls, standardizing formats, duplicate handling)
   - Transformations using Power Query
   - Exploratory analysis with Pivot Tables & slicers, dashboard creation

2. Power BI Dashboard
   - Dynamic visualization of data
   - Production Comparison Trend
   - Dynamic filtering: Top N, Day filters, machine/employee selection

3. Tableau Dashboard
   - Production trend visualization
   - Category-level rejected quantity and performance
   - Interactive drill-downs for department and employee

4. SQl(MYSQL)
   - Data extraction and filtering
   - Aggregating KPIs
   - Machine-wise and employee-wise rejection analysis
   - Department-wise manufacturing summary


### Technical Steps Followed

1. Data Cleaning & Transformation
   - Standardized date formats
   - Removed duplicate production entries
   - Created calculated fields for rejected %, wastage rate, etc.
   - Applied joins & relationships among tables
  
2. SQL Processing
   - Used GROUP BY, JOINS, CASE, Aggregate functions, and Window functions
   - Created datasets for dashboards

3. Power BI Development
   - Developed DAX measures for KPI calculations
   - Added interactive slicers (Top N, Date, Machine/Employee filters)
   - Designed story-driven dashboard

4. Tableau Visualization
   - Trend analysis
   - Rejection pattern mapping
   - Highlight tables for quick comparison  


### Dashboard Features
   - Manufactured Quantity : Shows the total units produced during the selected         period, reflecting overall production output.
     
   - Rejected Quantity : Displays the number of units that failed quality checks        and were rejected.
     
   - Wastage Quantity : Represents the count of materials wasted during production      process.
     
   - Processed Quantity : Indicates the units successfully processed after              manufacturing.
     
   - Employee wise Rejected Quantity : Highlights rejection counts contributed by       each employee to identify performance gaps.
     
   - Machine wise Rejected Quantity : Shows rejection distribution across machines      to detect maintenance or efficiency issues.
     
   - Departmentwise Rejected Quantity : Compares rejected units across departments      to analyze process-level performance.
     
   - Manufactured Quantity VS Rejected Quantity : Illustrates the relationship          between total production and rejection volume for quality assessment.
     
   - Production Comparison Trend : Tracks daily production and rejection trends        to observe fluctuations and identify patterns.

     
### Repository Structure

   📦 Manufacturing-Analysis-Project
│
├── 📄 README.md
├── 📊 PowerBI_Dashboard.pbix
├── 📊 Tableau_Workbook.twbx
├── 📈 Excel_Data.xlsx
├── 🗄 SQL_Scripts.sql
└── 📸 Dashboard_Screenshots/


### Key Insights

- Shruti Singh recorded the highest rejected quantity, indicating a need for         performance review.

- Machine C007 showed maximum rejections, suggesting machine maintenance             requirements.

- Woven Labels department produced the highest quantity but also showed noticeable   rejections.

- Overall rejection rate is very low compared to manufacturing output, indicating    good process efficiency.

- Trend chart shows fluctuating production peaks and dips that can be aligned with   shift timings or resource availability.    


### Tools Used

 - Excel
 - Tableau
 - PowerBI
 - SQl(MYSQL)


### Challenges and Solutions

1. Challenge: Inconsistent and Unclean Raw Data

Raw manufacturing data contained duplicates, missing values, and inconsistent formats.
Solution:
Performed data cleaning in Excel and Power Query, standardized date formats, removed duplicates, and validated fields before loading into BI tools.

2. Challenge: Difficulty in Identifying Rejection Patterns

Rejection data was scattered across multiple sources, making it hard to trace employee or machine-level issues.
Solution:
Used SQL to aggregate rejection metrics and created focused visuals in Power BI/Tableau to highlight top employees and machines causing rejections.

3. Challenge: Complex Calculations for KPI Metrics

KPIs like rejection percentage, wastage ratio, and processed quantity required multi-step calculations.
Solution:
Created DAX measures and calculated fields in Power BI/Tableau to ensure accurate and automated KPI computation.

4. Challenge: Large Dataset Slowing Down Dashboard Performance

Multiple tables and relationships caused slow refresh and load times.
Solution:
Optimized data model by removing unnecessary columns, using star schema, and applying query folding to improve performance.

5. Challenge: Limited Insights Across Departments and Time Periods

Stakeholders needed department-level trends and date-wise comparisons for better decision-making.
Solution:
Added interactive slicers (Top N, Day filters, department filters) and built comparison trend charts to provide deeper, dynamic insights.



### Future Enhancements

1. Integration of Real-Time Data Monitoring
Implement live data connections to track production, rejections, and machine performance in real-time.

2. Predictive Analytics for Rejection Forecasting
Use machine learning models to predict future rejection patterns and identify factors causing defects.

3. Automated Quality Alerts System
Build automated notifications when rejection quantity crosses a threshold for any employee or machine.

4. Advanced Root Cause Analysis Dashboard
Create drill-through pages to analyze reasons behind high rejections or wastage at a granular level.

5. Mobile-Optimized Dashboard View
Develop a mobile-friendly layout for supervisors to monitor KPIs from handheld devices on the shop floor.

6. Integration with ERP/MES Systems
Connect dashboards with ERP or Manufacturing Execution Systems (SAP, Oracle, etc.) for seamless data flow.

7. Time & Shift-Based Performance Comparison
Add shift-wise production and rejection insights for better workforce and scheduling optimization.

### Conclusion

This project demonstrates complete manufacturing performance monitoring using multiple BI tools for a 360° understanding of production, rejections, and efficiency. It helps identify process bottlenecks and supports data-driven decision-making in manufacturing operations.
