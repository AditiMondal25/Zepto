# 🛒 Zepto E-commerce SQL Data Analysis Project

## 📌 Project Overview
I designed and executed a comprehensive SQL analysis of Zepto's e-commerce inventory dataset, simulating real-world data analyst workflows from raw data exploration to business-focused insights. This project demonstrates my ability to derive actionable business insights from complex and messy retail data.

## 📁 Dataset Overview
I worked with a product inventory dataset containing:

- **sku_id**: Unique identifier for each product entry
- **name**: Product name as displayed to customers
- **category**: Product classification (Fruits, Snacks, Beverages, etc.)
- **mrp**: Maximum Retail Price
- **discountPercent**: Applied discount percentage
- **discountedSellingPrice**: Final price after discount
- **availableQuantity**: Inventory units available
- **weightInGms**: Product weight in grams
- **outOfStock**: Stock availability flag
- **quantity**: Units per package

## 🔧 Technical Implementation

### Database Architecture
I designed and implemented a PostgreSQL database schema optimized for e-commerce analysis:

```sql
CREATE TABLE zepto (
  sku_id SERIAL PRIMARY KEY,
  category VARCHAR(120),
  name VARCHAR(150) NOT NULL,
  mrp NUMERIC(8,2),
  discountPercent NUMERIC(5,2),
  availableQuantity INTEGER,
  discountedSellingPrice NUMERIC(8,2),
  weightInGms INTEGER,
  outOfStock BOOLEAN,
  quantity INTEGER
);
```

### Data Processing Pipeline
I developed a comprehensive ETL process that included:

1. **Data ingestion** with proper encoding handling
2. **Quality assessment** identifying incomplete and inconsistent records
3. **Currency normalization** converting paise to rupees for business reporting
4. **Data validation** removing invalid entries with zero pricing

## 📊 Analytical Methodology

### Exploratory Data Analysis
I conducted systematic data exploration to understand:

- Data completeness and quality across all columns
- Distribution of products across categories
- Inventory health metrics (in-stock vs out-of-stock ratios)
- Pricing distribution and discount patterns
- Identification of duplicate SKUs for same products

### Data Cleaning & Transformation
I implemented robust data cleaning procedures:

- Handled missing and inconsistent values
- Removed invalid records with zero pricing
- Standardized currency units across all financial metrics
- Validated weight and quantity measurements for accuracy

### Business Intelligence Development
I engineered SQL queries to extract actionable insights:

- **Value analysis**: Identified top 10 best-value products by discount percentage
- **Inventory optimization**: Flagged high-value out-of-stock items requiring restocking
- **Revenue forecasting**: Estimated potential revenue by product category
- **Pricing strategy**: Analyzed premium products with insufficient discounts
- **Category performance**: Ranked categories by average discount offerings
- **Cost efficiency**: Calculated price per gram to identify customer value propositions
- **Inventory segmentation**: Categorized products by weight for logistics planning
- **Supply chain analytics**: Measured total inventory weight by category

## 🎯 Key Findings & Business Impact

My analysis revealed several critical business insights:

1. **Discount Strategy Effectiveness**: Identified categories with most aggressive discounting
2. **Inventory Gaps**: Discovered high-margin products frequently out of stock
3. **Pricing Optimization Opportunities**: Found products with suboptimal discount structures
4. **Category Performance**: Quantified revenue potential across product categories
5. **Value Propositions**: Identified products offering best price-to-weight ratios

## 🛠️ Technical Skills Demonstrated

This project showcases my proficiency in:

- **SQL Database Design**: Schema creation and optimization
- **Data Wrangling**: Cleaning and transforming real-world messy data
- **Exploratory Data Analysis**: Systematic investigation of data patterns
- **Business Intelligence**: Translating data insights into actionable recommendations
- **Query Optimization**: Efficient SQL code for large dataset analysis
- **Data Visualization Preparation**: Structuring results for stakeholder reporting

## 📋 Project Deliverables

I produced a comprehensive SQL script containing:

- Database schema implementation
- Data quality assessment queries
- Data transformation procedures
- Business intelligence queries
- Executive-level summary metrics
- Category performance dashboards
- Inventory optimization recommendations

This project demonstrates my ability to handle complete data analysis workflows from raw data to business-ready insights, showcasing skills directly applicable to e-commerce and retail analytics roles.
