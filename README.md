## Hotel-Revenue-Data-Analysis-and-Visualization-Project

# Project Overview
This project provides a comprehensive end-to-end analysis of hotel revenue data. It involves data generation/collection, transformation using Power Query, advanced data modeling in Power BI, and the creation of an interactive dashboard to track key performance indicators (KPIs) such as ADR, RevPAR, and Occupancy %.

The analysis aims to help hotel managers understand booking trends, guest behavior, and financial performance across various branches and room types.

Key Features
Comprehensive Data Modeling: Implementation of a Star Schema for efficient reporting.

Advanced DAX Calculations: Custom measures and columns for deep insights into revenue and guest segmentation.

Guest Analysis: Segmentation of customers into categories like "High Spenders" and "Loyal Guests" based on frequency and revenue.

Dynamic Visualizations: Interactive cards, line charts for trend analysis, and matrix tables for granular data exploration.

Revenue Forecasting: Predictive analysis (built within the Power BI report) to estimate future booking trends.

Data Structure & Modules
The project was developed in structured modules:

Module 1: Data Preparation & Star Schema
Tables Created: Booking, Customer, Branch, RoomType, and Date.

Transformation: Initial formatting and loading into Power BI to establish a Star Schema relationship.

Enhancements: Added StayType (Day Use, Short Stay, Extended Stay, Long Stay) and RoomNightSold logic.

Module 2: Metric Definition (ADR & RevPAR)
Key Metrics:

ADR (Average Daily Rate): Calculated as Total Revenue / Room Night Sold.

RevPAR (Revenue Per Available Room): Calculated as Total Revenue / Total Rooms Available.

Occupancy %: The ratio of sold rooms to available rooms.

Visuals: Integrated KPI cards and trend lines to track these metrics over time.

Module 3: Advanced Guest Analytics
Data Merging: Combined TblRates and Tbl_Bookings using Power Query.

Customer Clustering: Developed logic to categorize guests:

First-Timer: < 5000 Revenue and 1 booking.

Loyal Guest: < 15000 Revenue and >= 3 bookings.

High Spender: >= 15000 Revenue.

RFM Scoring: Preliminary columns for Frequency, Spend, and Recency scores.

Technologies Used
Power BI: For data modeling, DAX, and visualization.

Excel/CSV: Source data management.

Power Query: For ETL (Extract, Transform, Load) processes.

Dashboard Preview
The dashboard includes:

Summary Matrix: Performance breakdown by month.

Trend Analysis: Line charts comparing ADR, RevPAR, and Occupancy % over time.

KPI Overview: High-level snapshots of total revenue and performance metrics.

Forecasting Page: (Internal to .pbix) Visual projections of future revenue based on historical data.

How to Use
Clone this repository.

Ensure the CSV files are in the designated directory if you wish to refresh the data.

Open HotelRevDashboard.pbix in Power BI Desktop to explore the interactive report.
