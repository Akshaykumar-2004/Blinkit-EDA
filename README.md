# Blinkit Sales Analysis

## Overview
This project involves a comprehensive analysis of Blinkit's sales data to understand performance, customer satisfaction, and inventory distribution. The goal is to identify key insights and opportunities for optimization using various KPIs and visualizations, primarily built using Python for EDA and planned for Power BI reporting.

## Business Requirements & Objectives
The analysis focuses on answering key business questions through specific KPIs and charts:
* **KPIs:**
    * Total Sales
    * Average Sales
    * Number of Items Sold
    * Average Customer Rating
* **Chart Requirements:**
    * Analyze the impact of item fat content on total sales.
    * Identify top-performing item types based on total sales.
    * Compare sales across outlets, segmented by fat content.
    * Evaluate how outlet establishment year influences total sales.
    * Analyze the correlation between outlet size and total sales.
    * Assess the geographic distribution of sales across different location types.

## Dataset
The analysis uses the `blinkit_data.csv` dataset, containing item details, outlet information, sales figures, and customer ratings.

## Methodology
1.  **Data Loading & Initial Inspection:** Loaded the dataset using Pandas and performed initial checks using `.head()` and `.info()`.
2.  **Data Cleaning:**
    * Standardized inconsistent values in the `Item Fat Content` column (e.g., 'LF', 'low fat', 'reg' mapped to 'Low Fat' or 'Regular').
    * Handled missing values: Dropped the `Item Weight` column due to a significant number of nulls.
3.  **Exploratory Data Analysis (EDA):**
    * Calculated overall KPIs: Total Sales, Average Sales, Number of Items, Average Rating.
    * Grouped data and aggregated sales by `Item Fat Content`, `Item Type`, `Outlet Location Type`, `Outlet Establishment Year`, and `Outlet Size`.
4.  **Visualization:** Created various plots using Matplotlib and Seaborn to visualize the findings:
    * Pie chart for Sales by Fat Content.
    * Bar chart for Sales by Item Type.
    * Stacked bar chart for Sales by Outlet Location and Fat Content.
    * Line chart for Sales by Outlet Establishment Year.
    * Pie chart for Sales by Outlet Size.
    * Bar plot for Sales by Outlet Location Type.

## Key Findings (Based on EDA)
* Low Fat items constitute the majority of sales compared to Regular items.
* 'Fruits and Vegetables' and 'Snack Foods' are the top-performing item types by sales volume.
* Tier 3 outlets generate the highest total sales, followed by Tier 2 and Tier 1.
* Sales peaked significantly for outlets established in 1998, with varying performance across other years.
* Medium-sized outlets account for the largest share of sales, followed by Small and High.

## Technologies Used
* Python
* Pandas
* NumPy
* Matplotlib
* Seaborn
* Jupyter Notebook
* Power BI (Planned for final dashboarding)
