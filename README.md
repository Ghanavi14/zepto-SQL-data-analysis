# zepto-SQL-data-analysis
This is a complete, real-world data analyst portfolio project based on an e-commerce inventory dataset scraped from Zepto — one of India’s fastest-growing quick-commerce startups. This project simulates real analyst workflows, from raw data exploration to business-focused data analysis.
📌**Project Overview**
The goal is to simulate how actual data analysts in the e-commerce or retail industries work behind the scenes to use SQL to:

✅ Set up a messy, real-world e-commerce inventory database

✅ Perform Exploratory Data Analysis (EDA) to explore product categories, availability, and pricing inconsistencies

✅ Implement Data Cleaning to handle null values, remove invalid entries, and convert pricing from paise to rupees

✅ Write business-driven SQL queries to derive insights around pricing, inventory, stock availability, revenue and more

📁**Dataset Overview**
 **Source:** Kaggle (scraped from Zepto's product listings)
- Each row = unique SKU (product variant)
- Duplicate names exist for different sizes/weights — mirrors real catalog data

**Key Columns:**
- sku_id — Unique product identifier
- name — Product name
- category — Product category
- mrp — Maximum Retail Price (converted from paise to ₹)
- discountPercent — Discount on MRP
- discountedSellingPrice — Final price after discount
- availableQuantity — Units in stock
- outOfStock — Boolean stock flag
🔧Project Workflow

### 1. Database & Table Setup
Created PostgreSQL table with appropriate data types and constraints.

### 2. Data Exploration
- Total record count
- Null value checks
- Distinct category identification
- In-stock vs out-of-stock comparison

### 3. Data Cleaning
- Removed rows with MRP or price = 0
- Converted prices from paise to rupees

### 4. Business Insights
- Top 10 best-value products by discount %
- High-MRP out-of-stock products
- Revenue estimation per category
- Price per gram (value-for-money analysis)
- Top 5 categories by average discount
- Product segmentation by weight (Low / Medium / Bulk)

---

## 🛠️ Tools Used
- **PostgreSQL**
- **pgAdmin**

🛠️**How to Use This Project**
1. Clone this repo
2. Open `zepto_file.sql` in pgAdmin
3. Create a database and run the SQL file
4. Import the CSV dataset (save as UTF-8 if needed)
