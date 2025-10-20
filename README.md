# Transportation Cost Optimization App

# Sample Data
Download sample data file from  https://drive.google.com/file/d/1WERrd0WxfI18X_XIBe6NyAMGwle-LbIy/view?usp=sharing

# Overview
A Streamlit web application that solves transportation cost optimization problems using linear programming with PuLP. The app minimizes transportation costs by optimally allocating shipments from warehouses to customers.

# App link: <a href="https://prescriptive-analytics-mdrgm8e64jj7sxy62nmaf3.streamlit.app/" target="_blank">Open Transportation Cost Optimization App</a>

# Features
Cost Optimization: Uses linear programming to minimize transportation costs

Multiple Warehouse Support: Handles GIR, GIR II, KSR4, LKDRM2, RSDSH, SLKPY warehouses

Dynamic Freight Rates: Calculates rates based on distance and warehouse

Data Visualization: Displays optimization results and cost comparisons

File Upload: Supports CSV and Excel file inputs

# How It Works

## Input Data Requirements

The app expects a file with these columns:

CustomerName (Party Name)

Plant (Warehouse)

TargetQuantity (Net Weight)

FreightRate

Distance

# Optimization Process

Data Preprocessing: Cleans and standardizes input data

Freight Calculation: Applies dynamic freight rates based on:

Distance thresholds (40km)

Warehouse-specific rates

Linear Programming: Uses PuLP to solve transportation problem

Cost Comparison: Shows before/after optimization costs

# Freight Rate Logic

GIR/GIR II: Fixed rate of 2.9

KSR4: Fixed rate of 2.5

Other Warehouses:

≤40km: Fixed rate of 100

40km: Rate of 2.5 per km

# Usage

Upload Data: Use the sidebar to upload CSV/Excel file

Select Party: Choose a customer from dropdown

Run Optimization: Click "Submit" to calculate optimal allocation

View Results: See cost savings and allocation plan

# Output

Optimal quantity allocation from each warehouse

Total transportation cost after optimization

Cost comparison with original allocation

Percentage cost reduction

# Technical Stack

Backend: PuLP, Pandas, NumPy

Frontend: Streamlit

Optimization: Linear Programming


# Author
Vikrant Nikunj - Data Science Enthusiast

Built with Streamlit and PuLP for efficient transportation cost optimization
