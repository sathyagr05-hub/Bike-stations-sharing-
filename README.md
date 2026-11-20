# 🚲 Bike Sharing Data Analysis using Power BI

## 📌 Project Overview

This project focuses on analysing bike-sharing station data using Microsoft Power BI. The main objective is to explore bike availability, station capacity, city-wise distribution and station status to generate meaningful insights that support better bike-sharing operations.

## 🎯 Project Objectives

- Import and explore the bike-sharing dataset in Power BI.
- Clean and transform data using Power Query.
- Build a logical data model using Fact and Dimension tables.
- Create relationships between Fact and Dimension tables.
- Develop DAX measures and calculated columns where required.
- Design interactive charts and dashboards.
- Analyse bike availability and station capacity across different cities.

## 🛠️ Tools & Technologies

- Microsoft Power BI
- Power Query
- DAX (Data Analysis Expressions)
- Microsoft Excel

## 📂 Dataset Description

The dataset contains information about bike-sharing stations, including:

| Column Name | Description |
|---|---|
| Station ID | Unique station identification number |
| Station Name | Name of the bike station |
| Address | Station location |
| Position | Latitude and longitude |
| Banking | Banking facility availability |
| Bonus | Bonus station information |
| Status | Station operating status |
| Contract Name | City name |
| Bike Stands | Total station capacity |
| Available Bike Stands | Available docking stands |
| Available Bikes | Number of available bikes |
| Last Update | Last updated date and time |

## 🧹 Data Cleaning & Transformation

Data preparation was performed using Power Query.

- Checked column names and data types.
- Removed unnecessary columns where required.
- Checked for missing and duplicate records.
- Standardised column formats.
- Prepared the data for modelling and analysis.

## 🏗️ Data Modelling

A logical data model was designed using a Star Schema approach.

### Fact Table – Fact_BikeAvailability

Stores measurable information:

- Station Key
- City Key
- Status Key
- Bike Stands
- Available Bike Stands
- Available Bikes
- Last Update Date

### Dimension Tables

| Dimension Table | Description |
|---|---|
| DimStation | Stores station details |
| DimCity | Stores city information |
| DimStatus | Stores station status |
| DimDate | Stores date, year, month and quarter information |

### Relationships

Relationships connect the Fact Table with the Dimension Tables using matching key columns.

- DimStation → Fact_BikeAvailability
- DimCity → Fact_BikeAvailability
- DimStatus → Fact_BikeAvailability
- DimDate → Fact_BikeAvailability

The intended relationship type is **One-to-Many (1:*)**, with dimension tables on the one side and the fact table on the many side.

## 📊 Power BI Visualizations

The report includes the following visualisation pages:

- **KPI Cards:** Display important summary values.
- **Bar Chart:** Compare values across categories.
- **Column Chart:** Present category-wise comparisons.
- **Pie Chart:** Show data distribution.
- **Line Chart:** Display data trends.
- **Donut Chart:** Represent proportions.
- **Map:** Show station locations geographically.
- **Dashboard:** Bring key visuals together in one report.

## 📈 Key Analysis Areas

- Total number of bike stations.
- Total bike stands and available bikes.
- City-wise station distribution.
- Station operating status.
- Availability of bikes across stations.
- Station capacity and available docking stands.
- Geographical distribution of bike stations.

## 💡 Key Learnings

Through this project, I gained practical experience in:

- Importing and exploring datasets in Power BI.
- Cleaning and transforming data using Power Query.
- Understanding Fact Tables and Dimension Tables.
- Creating relationships using primary and foreign keys.
- Building a logical data model.
- Creating interactive visualisations.
- Developing dashboards to communicate insights.

## 🏁 Conclusion

This Bike Sharing Data Analysis project helped me understand how to transform raw data into meaningful visual insights using Power BI. It improved my knowledge of data cleaning, data modelling, relationships and dashboard development. This project is an important step in building my Data Analytics portfolio.

---

**Project Type:** Data Analytics | Business Intelligence

**Tool:** Microsoft Power BI

**Created as part of my Data Analytics learning journey.**
