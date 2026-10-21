# Assignment-1-Power-BI-Data-Modelling-And-Transformation
Power BI Assignment
### 1. Data Import and Preparation
- Imported all three CSV files into Power Query.
- Retained the first 500 rows from List of Orders.
- Converted Order Date to Date format.
- Changed Amount and Target to Fixed Decimal Number.

### 2. Data Transformation
- Standardized CustomerName using proper case.
- Combined City and State into a new Location column.
- Created *Profit Margin* using:

  Profit Margin = Profit / Amount

- Created *Profit Status* based on profit values:
  - *Profit:* Profit > 0
  - *Loss:* Profit < 0
  - *Break-Even:* Profit = 0

### 3. Data Cleaning
- Checked for missing and null values.
- Identified and reviewed duplicate records.
- Sorted orders by Order Date in descending order.
- Filtered orders belonging to Tamil Nadu.

### 4. Data Merging
- Merged List of Orders and Order Details using Order ID.
- Applied a *Left Outer Join* to create Orders Data.

### 5. Data Aggregation
Used Power Query's *Group By* feature to calculate:

- Number of order-detail rows per Order ID.
- Average Profit by Category.
- Total Amount by Sub-Category.
- Total sales Target by month.

### 6. Data Modeling
Created relationships based on:

- *Order ID:* List of Orders → Order Details (One-to-Many)
- *Category:* Order Details ↔️ Sales target (potentially Many-to-Many)

A separate Category dimension is recommended for a more reliable production data model.

## Key Skills Demonstrated

- Data Import and Data Type Conversion
- Data Cleaning and Duplicate Detection
- Custom and Conditional Columns
- Data Merging and Filtering
- Grouping and Aggregation
- Data Modeling and Relationships

## Conclusion
This project demonstrates essential *ETL (Extract, Transform, Load)* techniques in Power BI. It transforms raw sales data into structured datasets suitable for further analysis, visualization, and business reporting.

This project demonstrates essential *ETL (Extract, Transform, Load)* techniques in Power BI. It transforms raw sales data into structured datasets suitable for further analysis, visualization, and business reporting.
