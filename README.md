🚀 Project Overview
This project demonstrates an end-to-end modern data analytics pipeline built using Microsoft Fabric, implementing the Medallion Architecture (Bronze → Silver → Gold) to transform raw movie industry data into meaningful business insights.

The solution analyzes India’s major film industries (Bollywood, Tollywood, Kollywood, Mollywood, and Sandalwood) to understand:
      Worldwide box office performance
      Budget distribution by industry
      Movie ratings trends over time
      Top performing movies by revenue

The project highlights how data engineering and BI can be combined using Microsoft Fabric, Lakehouse, Warehouse, Dataflow Gen2, and Power BI to create a scalable analytics solution.

🏗 Architecture – Medallion Data Pipeline

This project follows the Medallion Architecture, widely used in modern data platforms like Microsoft Fabric, Databricks, and Azure.

Raw CSV Data
     │
     ▼
Bronze Layer (Lakehouse)
     │
     ▼
Silver Layer (Dataflow Gen2 Transformation)
     │
     ▼
Gold Layer (Semantic Model + Power BI Dashboard)
🥉 Bronze Layer – Raw Data Ingestion (Lakehouse)

The pipeline begins by ingesting 5 CSV datasets containing movie information.

          Data Sources
          Movie titles
          Industry information
          Budget details
          Worldwide collections
          IMDb ratings

These CSV files are ingested into the Microsoft Fabric Lakehouse, which acts as the Bronze Layer storing raw, unprocessed data.

Purpose of this layer:
        Preserve raw source data
        Enable scalable storage
        Maintain historical records

🥈 Silver Layer – Data Transformation

The raw data is processed and transformed to prepare it for analytics.

Steps Performed
      1️⃣ Copy Data Pipeline - Data is moved from the Lakehouse (Bronze) to the Warehouse using a Copy Data pipeline.
      2️⃣ Dataflow Gen2 Transformation - Data cleansing and transformation performed, Missing values handled, Data types standardized, Tables appended into a single consolidated dataset
The result is a clean and structured dataset, which acts as the Silver Layer.

⭐ Data Modeling – Semantic Model
A Power BI Semantic Model was built on top of the transformed data using Star Schema modeling.

Fact Table
Movie Performance
Dimension Tables
Industry
Movie Title
Year
Ratings

This structure improves:
Query performance
Scalability
Analytical flexibility

🥇 Gold Layer – Business Intelligence (Power BI)

The final layer is the Power BI Report, which delivers actionable insights.

Key KPIs
💰 Total Worldwide Collection
🎬 Total Movie Budget
⭐ Average IMDb Rating

Analytical Insights

✔ Industry-wise box office performance
✔ Budget distribution across film industries
✔ IMDb rating trends over years
✔ Top performing movies by revenue
✔ Dynamic Top N movie analysis

Interactive filters allow users to explore different industries and movie performance metrics dynamically.

📊 Dashboard Highlights
The Power BI dashboard provides:
Industry revenue comparison
Budget distribution by industry
IMDb rating trends
Top revenue generating movies
Interactive Top N movie analysis
This helps stakeholders understand which film industries generate the highest box office returns and how ratings influence performance.

🛠 Tech Stack
Technology	Purpose
Microsoft Fabric	Data platform
Lakehouse	Bronze layer storage
Fabric Warehouse	Data processing layer
Dataflow Gen2	Data transformation
Copy Data Pipeline	Data movement
Power BI Semantic Model	Data modeling
Power BI	Visualization

📈 Business Value

This solution demonstrates how organizations can: Build modern analytics platforms using Microsoft Fabric
Implement Medallion Architecture for scalable data pipelines
Transform raw datasets into interactive business intelligence dashboards
Enable data-driven decision-making in the entertainment industry

⭐ Why This Project Stands Out
This project showcases both Data Engineering and BI skills, including:

✔ Microsoft Fabric Data Engineering
✔ Medallion Architecture Implementation
✔ Data Pipeline Development
✔ Dataflow Gen2 Transformations
✔ Star Schema Data Modeling
✔ Power BI Dashboard Design

📬 Connect With Me

If you're interested in Data Analytics, Power BI, or Microsoft Fabric solutions, feel free to connect and collaborate.
