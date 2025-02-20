# Warehouse-Inventory-Turnover-Analysis
## Overview

This project performs an in-depth **Warehouse Turnover Analysis** by analyzing inventory data, identifying key performance metrics, and providing insights into product behavior and future stock forecasts.

## Features

- **Data Preparation:**

  - Load and clean inventory data.
  - Handle missing restock dates using forward-fill.

- **Inventory Metrics Calculation:**

  - **Stock Turnover:** Sales per unit of stock (measures how quickly inventory is sold).
  - **Stock-to-Sales Ratio:** Measures how much stock exists relative to sales.

- **Product Categorization:**

  - Identify **slow-moving** and **high-demand** products.
  - Detect **excess inventory** outliers using the Interquartile Range (IQR) method.

- **Advanced Analytics:**

  - **Correlation Analysis:** Identify relationships among inventory metrics using a heatmap.
  - **Clustering Analysis:** Group products using KMeans clustering based on inventory and sales behavior.
  - **Time-Series Forecasting:** Predict future inventory levels using linear regression.

- **Visualization Outputs:**

  - Correlation heatmap to identify key relationships.
  - Scatter plot for clustering product behavior.
  - Inventory time-series plot with future forecasts.

## Dependencies

Ensure the following Python libraries are installed:

```bash
pip install pandas numpy matplotlib seaborn scikit-learn
```

## Usage

1. **Prepare Data:** Ensure your dataset (`inventory_data.csv`) has the following columns:

   - `product_id`: Unique product identifier
   - `stock_level`: Current inventory level
   - `sales`: Number of units sold
   - `restock_date`: Date of restocking (nullable)

2. **Run the Notebook:** Execute the Jupyter Notebook to:

   - Clean and process data
   - Perform inventory turnover analysis
   - Visualize key insights

3. **Interpret Outputs:**

   - **Slow-Moving Products:** Products with low turnover.
   - **High-Demand Products:** Products with rapid sales relative to stock.
   - **Excess Inventory:** Outliers indicating overstocked products.

## Results

The analysis generates key outputs:

- Inventory summary with calculated KPIs.
- Identification of slow-moving and high-demand products.
- Visualization of inventory patterns and future stock forecasts.

## Example Outputs

1. **Inventory Summary:**

```
   product_id  total_stock  total_sales  stock_turnover  stock_to_sales_ratio
0           1        1500         300           0.20                5.00
1           2         200         400           2.00                0.50
```

2. **Forecast Plot:**
   A time-series chart showing past inventory levels and predicted future stock for the next 10 days.

## Customization

- Adjust the number of clusters in the KMeans algorithm.
- Modify the forecast period for longer-term projections.

## License

This project is open-source and available under the MIT License.

add folder structure, Installation & Setup and technologies used

