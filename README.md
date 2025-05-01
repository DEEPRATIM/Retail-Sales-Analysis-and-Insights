# Retail-Sales-Analysis-and-Insights

This project presents a comprehensive analysis of a US retail sales dataset covering office supplies, furniture, and technology using python. The goal is to uncover actionable insights to optimize profitability, pricing, discounting, and inventory strategies for a multi-region, multi-segment retailer.

🗂️ Dataset
* Source: US Retail Sales Dataset
* Rows: 9,994 transactions, Columns: 16 original features + engineered features (profit, loss, discount amount, etc.)
* Key fields: Order Id, Order Date, Ship Mode, Segment, Region, Category, Sub Category, Product Id, cost price, List Price, Quantity, Discount Percent

⚙️ Data Cleaning & Preprocessing
* Removed 507 orders with both zero cost and zero list price (invalid transactions)
* Converted date columns and fixed missing values (e.g., Ship Mode)
* Segmented orders into main and outlier clusters using IQR for robust analysis
* Engineered profit/loss and discount features for deeper insights

🔍 Exploratory Data Analysis (EDA)
* Univariate & Bivariate Analysis: Explored distributions, outliers, and clusters using boxplots, histograms, and pie/bar charts
* Category & Subcategory Profitability: Identified Technology as top profit drivers in outliers; Office Supplies as high-volume but low-margin in main cluster
* Loss Analysis: All top loss-making products are Office Supplies (Binders, Fasteners, Paper) with small per-unit losses compounding to large totals
* Geographic Trends: Major cities (NYC, LA, SF) dominate volume, but smaller cities (Lafayette, Jacksonville, Detroit) lead in profit per order
* Seasonality: MoM sales trends reveal strong Q4 peaks and notable year-on-year fluctuations
* Discount Impact: Higher discounts erode profit, especially for premium products and Furniture

💡 Key Business Insights
* Nearly half of all transactions are loss-making (mainly in Office Supplies); urgent review of pricing and discounting is needed
* Premium product outliers (Machines, Copiers) deliver 10–50× higher profit per order and are less vulnerable to discounts
* Targeted regional and seasonal strategies can maximize both volume and profit
* Binders, Fasteners, and Paper are the biggest loss drivers due to high sales volume and small negative margins

📝 Recommendations
* Revise pricing and discount policies for Office Supplies and Furniture to reduce loss-making orders
* Focus premium inventory and marketing in high-profit cities and during peak months (Q4)
* Discontinue or renegotiate loss-making SKUs to save costs and improve margins
* Monitor and optimize discounting for premium products to protect high-value margins

📈 Limitations & Next Steps
* No customer demographic or competitor pricing data included
* Analysis limited to 2022–2023 transactions
* Future work: Customer segmentation, inventory optimization, A/B testing for pricing, extended time series forecasting

🛠️ Tools & Libraries
Python (pandas, numpy, matplotlib, seaborn)
Jupyter Notebook
