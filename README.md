# Interactive Sales Performance Dashboard

This project showcases two versions of an Interactive Sales Performance Dashboard developed using Power BI. 
The first version integrates a SQL Database (MySQL/PostgreSQL/SQL Server), and the second version uses Excel as the data source.
Both versions provide real-time data analysis, advanced data visualization, and insightful predictive analytics for sales performance tracking.

# Project Overview

The Interactive Sales Performance Dashboard is designed to visualize and analyze sales data across 
multiple dimensions, including:

* Total sales
* Sales by region
* Sales trends over time
* Profit margins and growth rates
* Forecasting and predictive analysis
* Geospatial insights via maps
  
## Features
* SQL Version: DirectQuery integration for real-time data updates.
* Excel Version: Data pulled from Excel files for smaller-scale projects.
* Advanced Visualizations: KPI cards, trend analysis, line charts, bar charts, and maps.
* DAX Calculations: Custom metrics like total sales, profit margin, and growth rate.
* Drill-through and Slicers: Interactive filtering and detailed insights.
* Forecasting: Predicted sales trends based on historical data.
  
## Table of Contents
1.Prerequisites
2.Setup Instructions
3.SQL Version - Setup
4.Excel Version - Setup
5.Power BI Design
6.Pictures
7.Features
8.How to Run the Project
9.Contributing
10.License

## Prerequisites
Before you start, ensure you have the following installed on your machine:

For SQL Version:
* Power BI Desktop: For designing and visualizing the dashboard. You can download it here.
* SQL Server/MySQL/PostgreSQL: You need a database server installed and running to connect to Power BI.
* SQL Database: A pre-configured SQL database with sales data (you can use the provided sample dataset or create your own).

For Excel Version:
* Power BI Desktop: Same as above.
* Excel: The sales data should be stored in an Excel file. The project uses sample data, which
  you can replace with your own.

## Setup Instructions

1. Clone the Repository
Clone the repository to your local machine using the following command:
git clone https://github.com/yourusername/interactive-sales-dashboard.git

2. Open Power BI Desktop
Open Power BI Desktop to import the data source and start designing the dashboard.

SQL Version - Setup
1. Prepare the SQL Database
* Set up your preferred SQL database (MySQL, PostgreSQL, or SQL Server).
* Create a new database and import the provided sales_data.sql file (or use your own data).

Sample SQL for creating a sales database:
CREATE DATABASE sales_db;
USE sales_db;

CREATE TABLE sales (
    id INT PRIMARY KEY AUTO_INCREMENT,
    region VARCHAR(255),
    product VARCHAR(255),
    sales_amount DECIMAL(10,2),
    sales_date DATE
);

INSERT INTO sales (region, product, sales_amount, sales_date)
VALUES 
('North', 'Product A', 1500.00, '2024-01-01'),
('South', 'Product B', 1200.00, '2024-01-02');

2. Connect Power BI to SQL Database
~ Open Power BI Desktop.
~ Click on Home → Get Data → SQL Server (or MySQL/PostgreSQL).
~ Enter the server name and database name, then click OK.
~ Load the data into Power BI for visualization.

3. Configure Data Model
~ Import the necessary tables (sales, products, regions, etc.).
~ Ensure relationships are correctly set up between the tables.

4. Design the Dashboard
~ Use Power Query to clean and transform the data.
~ Use DAX to create calculated columns and measures for sales metrics.
~ Create visualizations (e.g., line charts, bar charts, KPI cards).
~ Use DirectQuery for real-time updates from SQL.

Excel Version - Setup
1. Prepare the Excel File
~ Ensure your sales data is structured in Excel (e.g., columns for Region, Product, Sales Amount, Sales Date).
~ Save the file as sales_data.xlsx.

2. Import Excel Data into Power BI
~ Open Power BI Desktop.
~ Click on Home → Get Data → Excel.
~ Select your sales_data.xlsx file and load the data.

3. Design the Dashboard
~ Similar to the SQL version, use Power Query for cleaning and transforming the data.
~ Create DAX measures for metrics such as total sales, profit margins, and growth rates.
~ Design visualizations (e.g., bar charts, line charts, maps).

## Power BI Design
The dashboard includes the following:

* Main Dashboard: Displays an overview of total sales, sales by region, and profit margins.
* Geospatial Insights: Uses maps to visualize sales by region.
* Sales Trends: Line charts showing sales over time.
* KPI Cards: For metrics like total sales, average sales per region, and growth rate.
* Forecasting: DAX-powered forecast models for future sales.

### Pictures
Here are some screenshots of the Interactive Sales Performance Dashboard:

# Database Intergration:


<img width="945" alt="Screenshot 2025-01-12 182102" src="https://github.com/user-attachments/assets/f04a97e5-3f1a-4854-944b-9c91ddefa567" />

<img width="949" alt="Screenshot 2025-01-12 182120" src="https://github.com/user-attachments/assets/3b81969c-63b4-4dc0-8f59-af62837f36e3" />


# Excel intergration:


<img width="944" alt="Screenshot 2025-01-12 182214" src="https://github.com/user-attachments/assets/eab4194a-19c9-4d88-9110-135311a83bc5" />

<img width="948" alt="Screenshot 2025-01-12 182241" src="https://github.com/user-attachments/assets/00f98cd7-3f56-4aed-8f45-5ecf3150a4f8" />

How to Run the Project

* After setting up the data source (SQL or Excel), open Power BI Desktop.
* Load the data and configure the dashboard as per the instructions above.
* Explore the various filters, slicers, and drill-through features to interact with the dashboard.
* Use the forecasting model to predict future sales trends.

## Contributing
Feel free to contribute to this project by following these steps:

## Fork the repository.

Create a new branch (git checkout -b feature-name).
Make your changes and commit (git commit -am 'Add new feature').
Push to the branch (git push origin feature-name).
Submit a pull request.

## License
This project is licensed under the MIT License 




