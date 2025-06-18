# VENDOR-PERFORMANCE-DATA-ANALYTICS-USING-PYTHON-SQL-POWER-BI
 Analyzed vendor performance using Python, SQL, and Power BI to identify profit leaks, inventory issues, and top-performing suppliers. Delivered actionable insights through EDA, dashboards, and a detailed report to support data-driven business decisions.

DATA SETS- https://1drv.ms/f/c/8e1a8ca8b0dd53d5/EtbEJQkHdaBBj4Do6zeXWvkBwZGXntumAyV6ygyn4Au51Q?e=re3MW0

Overview
This project focuses on analyzing vendor performance data to help a business improve its inventory management, profitability, and vendor relationships. Using real-world sales, purchase, and freight data, we performed data ingestion, cleaning, exploratory data analysis (EDA), and built a comprehensive Power BI dashboard to deliver actionable business insights.

Business Problem
Retail and wholesale businesses often struggle with:
-Inventory that doesn’t move
-Vendors with low performance or profit
-Unbalanced reliance on a few suppliers
-High logistics/freight costs
-Poor correlation between cost and profit

Objective: To analyze vendor performance and sales efficiency to guide smarter business decisions around procurement, pricing, and inventory management.

Tools & Technologies
-Python (Pandas, SQLite, Jupyter Notebooks, SQLAlchemy)
-Power BI (for interactive dashboarding)
-Jupyter Notebook (for EDA)
-PDF Report (executive summary)
-SQLite (lightweight relational database)

Data Sources
CSV files containing:
-Purchase records
-Sales records
-Freight invoices
-Pricing data

Key Steps Performed
1. Data Ingestion
-Used ingestion_db.py to load all raw CSVs into a local SQLite database.
-Logged every file processed to ensure traceability.

2. Data Modeling & SQL Queries
-Wrote optimized SQL queries (in get_vendor_summary.py) to:
Merge sales, purchases, and freight data
-Compute sales volume, gross profit, excise tax, and freight costs
-Derive new metrics like Profit Margin, Stock Turnover, Sales to Purchase Ratio

3. Data Cleaning
-Removed whitespace, converted dtypes
Filled missing values
Removed vendors/products with:
Zero sales quantity
Negative or zero gross profit and profit margins

4. Exploratory Data Analysis
-Conducted in Exploratory Data Analysis.ipynb and Vendor Performance Analysis.ipynb, including:
Distribution of sales and purchase data
Detection of outliers
Correlation studies between pricing, sales, and margin
Filtering and segmenting for deep-dive analysis

5. Interactive Dashboard (Power BI)
-Created a .pbix file with slicers by vendor, brand, region
Visuals for:
Sales & profit over time
Vendor-wise comparison
Inventory turnover and freight efficiency

6. Insights & Recommendations
See PDF report: Vendor Performance Report.pdf

Key Insights
-Inventory Inefficiencies
Products with zero sales despite high purchase costs.
Inventory holding capital worth $2.71 million in unsold stock.

 Profit Analysis
-Negative profit margins for some products (min -₹52,000+), likely due to discounts or poor pricing.
-High-margin vendors often have lower sales, signaling pricing or marketing gaps.

Freight Cost Variability
-Freight charges ranged from ₹0.09 to ₹2.5 lakhs — highlighting possible supply chain inefficiencies.

Vendor Risk
-10 vendors contribute over 65% of all purchases — indicating a dependency risk.

 Bulk Purchase Advantage
-Vendors purchasing in bulk enjoyed 72% lower unit cost — an opportunity to optimize buying strategies.

 Actionable Suggestions
-Diversify vendor partnerships.
-Adjust pricing for low-selling, high-margin brands.
-Optimize slow-moving inventory via discounts or better planning.
-Promote vendors with high sales but low profit to adopt cost-efficiency.

Research Questions Answered
-Which brands need promotional or pricing adjustments?
-Who are the top vendors by sales and purchase value?
-How does bulk buying affect unit cost?
-Which vendors have the lowest inventory turnover?
-How do profit margins differ between high- and low-performing vendors?

Is the difference in profit margins statistically significant?
 Statistical Analysis
-Performed hypothesis testing to compare high- and low-performing vendor profit margins.

Final Thoughts
This project shows how organized data and clear analysis can help solve real business problems. It covers everything from writing code and using databases to exploring data.
