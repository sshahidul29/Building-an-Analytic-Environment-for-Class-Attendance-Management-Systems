## Overview

This project aims to empower our Educational Institute client with data-driven insights and decision-making capabilities by providing a robust data infrastructure and actionable analytics. It involves integrating, cleaning, and structuring data, and creating the analytical model for informed decision-making.

## Contributions
-
-
-
## Software requirements:
- MS SQL Server, SSMS, SSIS, and Visual Studio
- Windows OS

## Data Management and Processes
Data Management and Processes involved with
- Data Governance
- Data Quality and Validation
- Data Retention Policy
- Master Data Management

## System Development Life Cycle (SDLC)
- Agile Kanban Methodology

## Enterprise Data Warehouse was built in MS SQL Server using SSMS

- Performed business requirement gathering, documentation and profiling of available data.
- Collaborated with the project team to identify and document source-to-target mapping.
- Created the opportunity/stakeholder Matrix (it helps identify which business groups should be invited to the collaborative design sessions for each process-centric row).
- Constructed a Bubble Chart for communicating data models to a non-technical audience. 
- Created Bus Matrix (composition of Business process, Granularity, Facts, Fact Tables, and Dimensions).
- Designed and implemented Enterprise Data Warehouse (EDW) using Ralph Kimball’s Dimensional Modelling Approach.
- Created and configured Staging, EDW, and Control Framework databases on MS SQL Server. 
![Class Attendance](https://github.com/sshahidul29/Building-an-Analytic-Environment-for-Class-Attendance-Management-Systems/blob/main/Figures/ClassEDW.PNG)  
Figure 1: Class Attendance Star Schema

## ETL Pipeline was built in Visual Studio using SSIS

- Produced ETL Mapping and Transformation Rules and data Quality documentation for the project.
- Developed and tested ETL processes/programs necessary to extract data from different data sources, Transformed and cleansed the data, and loaded it into a Staging database and Staging to Data Warehouse, using connection managers like OLE DB, Excel, Flat file, and ADO.NET.
- Created a metric table for an audit of Source Count, and Destination Count Staging database, and Pre, Current, Post, Type1, and Type2 Counts for EDW using the Control framework database.
- Design and Implement Ralph Kimball slowly changing dimension (SCD) Type 1 and 2.
- Troubleshooting and root cause analysis activities to fix bugs in the data integration process.
- Scheduled and monitored SQL Server Agent jobs to run ETL SSIS packages to move data.
 
 ![Class Attendance](https://github.com/sshahidul29/Building-an-Analytic-Environment-for-Class-Attendance-Management-Systems/blob/main/Figures/ClassETL3.PNG) 

 Figure 2: Control-flow diagram for ETL Pipeline

   ![Class Attendance](https://github.com/sshahidul29/Building-an-Analytic-Environment-for-Class-Attendance-Management-Systems/blob/main/Figures/ClassETL1.PNG) 

 Figure 3: Data-flow diagram of ETL Pipeline for Student dimension

  ![Class Attendance](https://github.com/sshahidul29/Building-an-Analytic-Environment-for-Class-Attendance-Management-Systems/blob/main/Figures/ClassETL2.PNG) 

Figure 4: Data-flow diagram for Incremental load of ETL Pipeline for FactClassAttendance

 ![Class Attendance](https://github.com/sshahidul29/Building-an-Analytic-Environment-for-Class-Attendance-Management-Systems/blob/main/Figures/ClassETL4.PNG) 

Figure 5: Control-flow diagram for ETL Pipeline to automate the system through SQL Server Agent


