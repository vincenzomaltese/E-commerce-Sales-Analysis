# The Office Store - E-commerce Sales Analysis

This repository contains a Tableau project analyzing sales data for a fictional e-commerce company called **The Office Store**. The company specializes in **Office Supplies, Furniture, and Technology** products, serving General Consumers, Corporate, and Home Offices across the United States.

## Project Overview

- **Goal**: Provide insights into key performance metrics such as **Sales**, **Profit**, **Top-Performing Products**, **Customer Segments**, and **Regional Trends**.
- **Dataset**: The data is from a fictional online store with no physical locations. Products are manufactured in the US and Canada, and shipped to customers across the US.
- **Time Frame**: The dataset spans orders from **2016 to 2019**.

## Data Model

The project uses a star schema consisting of one **Fact** table (`FactOrder`) and several **Dimension** tables:

- **FactOrder**: Contains order-level information such as Order Date, Revenue, Units, Quantity, Cost, and Ship Date.
- **dimCustomer**: Stores customer details (Name, Email).
- **dimLocation**: Provides location data (State, Abbreviation, Region).
- **dimProduct**: Holds product information (Name, Category, SubCategory, SKU).
- **dimShipping**: Describes shipping methods and types.
- **dimPromo**: Contains promotional details (Promo Code, Campaign, Amount).

These tables were provided as Excel files, joined in Tableau to create a single, integrated dataset for analysis.

## Dashboards

### 1. Sales Dashboard
- **Key Metrics**:  
  - **Total Sales** (USD)  
  - **Total Profit** (USD)  
  - **Profit Ratio** (%)  
  - **Order Count**  
  - **Average Order Value (AOV)**  
  - **Average Days to Ship**  
- **Profitability Scatter Plot**: Shows **Profitable vs. Unprofitable** customers across different sales levels.  
- **Sales by Category/Subcategory**: Highlights which categories and subcategories drive the most revenue.  
- **Profit by Month**: Allows users to focus on specific product categories (e.g., Technology) to identify seasonal or monthly trends.

![Performance by Location on Tableau Public](https://github.com/vincenzomaltese/The-Office-Store-E-commerce-Sales-Analysis/blob/main/images/Sales_Dashboard.jpg)

**Explore Dashboard**: [Sales Dashboard on Tableau Public](https://public.tableau.com/app/profile/vincenzo.maltese1450/viz/CaseStudyTheOfficeStore-SalesDashboard/SalesDashboard)
### 2. Performance by Location
- **Top 10 States by Sales**: Visualizes which states generate the highest revenue.  
- **Geographical View**: Uses a map to show **Regions** (Northeast, South, Midwest, West) and the corresponding performance.  
- **Top 10 Performing Products**: Treemap highlighting sales and profitability status.

![Performance by Location on Tableau Public](https://github.com/vincenzomaltese/The-Office-Store-E-commerce-Sales-Analysis/blob/main/images/Performance%20by%20Location.jpg)

**Explore Dashboard**: [Performance by Location on Tableau Public](https://public.tableau.com/app/profile/vincenzo.maltese1450/viz/CaseStudyTheOfficeStore-PerformancebyLocation/PerformancebyLocation)

## Key Insights

1. **Top-Performing States**  
   - California leads in sales, followed by New York and Texas.  
   - Regional performance can be quickly compared via the color-coded map.

2. **Most Profitable Categories**  
   - **Technology** products appear to drive the highest sales overall.  
   - Office Supplies and Furniture also contribute significantly but have varied profit margins.

3. **Customer Profitability**  
   - The scatter plot shows a cluster of **unprofitable** customers with lower sales.  
   - Larger orders (above \$15K) tend to be more profitable, though there are exceptions.

4. **Shipping and Promotions**  
   - Faster shipping methods correlate with slightly higher costs but may improve customer satisfaction.  
   - Promo usage patterns can be analyzed to optimize future campaigns.

5. **Seasonality**  
   - Certain months (e.g., November) show spikes in profit, particularly for Technology products.

## Tools and Technologies

- **Tableau**: For data visualization, dashboard creation, and interactive analysis.  
- **Excel**: Data storage and initial data cleaning.  

## How to View or Reproduce

1. **Clone the Repository**  
   ```bash
   git clone https://github.com/yourusername/office-store-tableau.git
