📊 Power BI Data Modeling Project
🚀 Project Overview

This project demonstrates the process of preparing, modeling, and visualizing data in Power BI using a Star Schema approach. The dataset includes Sales and Returns fact tables with supporting dimension tables (Date, Customer, Product, Region).

The final report provides insights into Revenue by Customer Segment, Region, Category, and Fiscal Year.

🛠 Steps Completed
1. Data Import

Imported datasets:

Sales_Fact

Return_Fact

Customer_Dim

Product_Dim

Region_Dim

Date_Dim

2. Data Cleaning & Transformation

Removed blanks and duplicates

Applied correct data formats (e.g., Date, Currency, Whole Number, Text)

Renamed and standardized column headers

Set key columns for relationship building

3. Data Modeling

Created a Star Schema with fact and dimension tables

Defined relationships:

Sales_Fact → Date_Dim

Sales_Fact → Customer_Dim

Sales_Fact → Product_Dim

Sales_Fact → Region_Dim

Return_Fact → Sales_Fact (via SalesID)

Used single-direction filters (dimension → fact)

Created inactive relationship between Return_Fact and Date_Dim (ReturnDateKey) for simulation of scenarios

4. Data Formatting & Hierarchies

Applied Data Categories (e.g., Geo fields like Region)

Created Hierarchies (e.g., Date Hierarchy → Year → Quarter → Month → Day)

5. Reporting (Matrix Visualization)

Built a Matrix visual:

Rows → Category, Region

Columns → Fiscal Year

Values → Sum of Revenue

Provides Revenue breakdown by Customer Segment, Region, and Fiscal Year

⚖️ Filter Management

Single-direction filters maintained for clarity and performance

Bidirectional filters avoided, except where justified

Inactive relationships used for testing Returns analysis

🧑‍💻 How to Use

Open the .pbix file in Power BI Desktop

Explore the Data Model view to understand schema and relationships

Check the Report view for prebuilt visuals
