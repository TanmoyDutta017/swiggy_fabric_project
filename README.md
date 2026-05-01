# Swiggy Fabric Data Analytics Project

## Swiggy_Fabric_Report
![Reprort](https://github.com/TanmoyDutta017/swiggy_fabric_project/blob/main/Report.png)

## Data Pipeline

![Pipeline](https://github.com/TanmoyDutta017/swiggy_fabric_project/blob/main/Pipeline.png)

## Semantic Model
![Model](https://github.com/TanmoyDutta017/swiggy_fabric_project/blob/main/Semantic%20Model.png)

### 📌 Project Overview

This project demonstrates an end-to-end data engineering and analytics solution using Microsoft Fabric. It involves ingesting raw Swiggy delivery data, processing it through a Medallion-style architecture (Lakehouse to Warehouse), and delivering actionable insights via a Power BI dashboard.



### 🏗️ Architecture \& Workflow

The project follows a structured pipeline within the Swiggy\_Fabric\_Project workspace:



Data Ingestion (Lakehouse): Created swiggy\_lh to store raw CSV files.



Data Transformation (SQL): Performed data cleaning and schema definition using Spark/SQL within the Lakehouse environment.



Data Orchestration (Pipelines): Developed a Data Pipeline to move cleaned tables into the Swiggy\_DW (Data Warehouse). As seen in image\_4a5779.png, the pipeline successfully handles the ingestion of Date, Dish, Location, Restaurant, and Fact Order tables.



Semantic Modeling: Built a Star Schema relationship model connecting the Fact table to dimensions.



Visualization: Connected the semantic model to Power BI Desktop for advanced reporting.



### 📊 Dashboard Key Features

The final report (referenced in image\_4a573b.png) provides insights into:



Key Metrics: Total Sales (₹53.01M), Avg Order Value (₹268.51), and Total Orders (197.43K).



Trends: Monthly sales performance and Total Sales by Day Name.



Geographical Analysis: Top 15 states by sales (led by Karnataka and Uttar Pradesh).



Performance: Top 5 performing restaurants (KFC, McDonald's, etc.) and Food Type distribution (Veg vs. Non-Veg).



### 🛠️ Technical Stack

Platform: Microsoft Fabric



Storage: OneLake (Lakehouse \& Warehouse)



Data Movement: Fabric Data Factory (Pipelines)



Language: SQL (Data Cleaning)



Modeling: DAX (Data Analysis Expressions)



Visualization: Power BI Service \& Desktop



### 🗄️ Data Model

The semantic model (shown in image\_4a53a1.png) utilizes a Star Schema:



Fact Table: fct\_order



Dimension Tables: location, date, dish, and resturant.



Measure Table: A dedicated table created to house all DAX calculations for better organization and performance.



🚀 How to Use

Fabric Workspace: Ensure you have an active Microsoft Fabric capacity.



Data Load: Upload the CSVs to the Files section of your Lakehouse.



Run Pipeline: Execute the pipeline to populate the Warehouse.



Open Report: Use the .pbip or live connection to view the Swiggy\_Fabric\_Report.

## Tools Used

- **Microsoft Fabric**: Used for upload data in lakehouse, to create warehouse , semantic model and to publish end report.
- **Power BI Dekstop**: To create Swiggy_Fabric_Report.

## 🛡️License
This project is licensed under the MIT License. You are free to use, modify, and share this project with proper attribution.

## ⭐About Me

Tanmoy Dutta    
Regional Coordinator/MIS Executive  
📧Email: iamtanmoydutta@gmail.com   
🔗 [LinkedIn](https://www.linkedin.com/in/tanmoy-dutta-53996820b/)







