# Northwind Traders Global Sales & Operations BI Dashboard

## About This Project
I was given a challenge: take a raw dataset and turn it into a business intelligence solution that answers real executive questions. The dataset belonged to Northwind Traders, a global gourmet food supplier, and covered everything from customer orders and product categories to employee performance and shipping costs. Using Microsoft Power BI, I transformed 7 raw tables into a fully interactive 3-page executive dashboard.

## Tool Used
- Microsoft Power BI

## Dataset
The Northwind Traders dataset consists of 7 tables:
| Table | Description |
|-------|-------------|
| Orders | 831 records covering order dates, freight costs and shipper info |
| Order Details | Product quantities, unit prices and discounts per order |
| Customers | Global customer information including city and country |
| Products | 77 products across 8 categories with pricing and discontinued status |
| Categories | 8 product categories |
| Employees | 9 sales employees and their reporting structure |
| Shippers | 3 shipping companies |

## Data Model
I connected all 7 tables using 6 relationships in Power BI:
- Customers → Orders (CustomerID)
- Orders → Order Details (OrderID)
- Orders → Employees (EmployeeID)
- Orders → Shippers (ShipperID)
- Order Details → Products (ProductID)
- Products → Categories (CategoryID)

## DAX Measures Created
- Total Revenue
- Total Orders
- Average Order Value
- Total Discount
- Profit Margin %
- Average Freight Cost
- Average Delivery Days

## Dashboard Pages

### Page 1 — Sales & Revenue Overview
This page gives the executive team a high level view of overall business performance. It includes KPI cards for Total Revenue, Total Orders and Average Order Value, a line chart showing revenue trends from July 2013 to May 2015, and a bar chart revealing monthly seasonal patterns with April consistently emerging as the peak revenue month.

![Page 1 Screenshot](https://github.com/onyi-data/Northwind-Traders-Global-Sales-Operations-BI-Dashboard/blob/main/dash1.png?raw=true)

### Page 2 — Product & Category Intelligence
This page dives into product and category performance. It includes a bar chart of revenue by category, a treemap of top products by revenue, a donut chart comparing active vs discontinued products, and a table showing detailed product performance. Beverages emerged as the top revenue category at $267,868.18 while Côte de Blaye was the single highest revenue generating product.

![Page 2 Screenshot](https://github.com/onyi-data/Northwind-Traders-Global-Sales-Operations-BI-Dashboard/blob/main/dash2.png?raw=true)

### Page 3 — Regional, Operational & People Performance
This page covers regional insights, shipping efficiency and employee performance. It includes a world map of revenue by country, a bar chart of sales by employee, column charts comparing shipper costs and delivery speeds, and freight cost analysis by country. The USA was the top revenue market, Margaret Peacock was the top salesperson and Federal Shipping was the fastest and most cost efficient shipper.

![Page 3 Screenshot](https://github.com/onyi-data/Northwind-Traders-Global-Sales-Operations-BI-Dashboard/blob/main/dash3.png?raw=true)

## Filters
The dashboard includes 3 working filters synced across all 3 pages:
- Year
- Country
- Category

## Key Recommendations
- **Shipping Efficiency:** United Package is the slowest and most expensive shipper. Shift more shipments to Federal Shipping.
- **Discount Strategy:** Beverages is already the top category but receives the highest discounts. Reducing discounts could improve margins.
- **Freight Costs:** Austria has disproportionately high freight costs of $184.79 average. Shipping rates should be renegotiated.
- **Market Expansion:** Northwind Traders has no presence in Africa, Asia or Australia significant untapped markets.
- **Discontinued Products:** Discontinued products still contribute 14.61% of revenue. Replacements should be introduced before discontinuing existing ones.

## Files
- `Northwind_Traders_Dashboard.pbix` — Power BI Dashboard file
- `Northwind_Traders_Report.pdf` — Project Report

## Dashboard & Report Link
[https://drive.google.com/drive/folders/1Chz0p2D5nERgpBBYdx9qSf-K_av7iAUI?usp=drive_link]

## Contact
 | [onyiokereke10@gmail.com] | [https://www.linkedin.com/in/onyinye-okereke]
