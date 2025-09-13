# Sales Data Analysis - Lebanon & Jordan

A mini data analysis project to practice **pandas data preprocessing** and **data visualization** using matplotlib and plotly. This project analyzes sales data from a business operating in Lebanon and Jordan through both online and offline channels.

## Project Overview

This project focuses on:
- Data cleaning and preprocessing with pandas
- Exploratory data analysis (EDA) 
- Creating visualizations to understand sales patterns
- Extracting business insights from the data

The analysis covers sales performance across different countries, channels, products, and time periods to identify trends and opportunities.

## Dataset Description

The dataset contains sales records with the following columns:

### Order Information
- `order_id` - Unique identifier for each order
- `date` - Order date
- `year` - Year extracted from date
- `month` - Month extracted from date  
- `weekday_name` - Day of the week

### Customer & Geography
- `customer_id` - Customer identifier
- `country_code` - Country where sale occurred (Lebanon/Jordan)
- `customer_segment` - Customer classification

### Sales Details
- `channel` - Sales channel (online/offline)
- `sales_person` - Sales representative
- `units_sold` - Number of units sold
- `unit_price` - Original unit price
- `unit_price_usd` - Unit price in USD
- `discount_pct` - Discount percentage applied
- `total_amount` - Final order value

### Product Information
- `product_code` - Product identifier
- `product` - Product name/description
- `promotion_flag` - Whether promotion was applied
- `sales_volume_category` - Sales volume classification

### Commission
- `commission_percent` - Commission rate
- `commission_amount` - Commission earned

## Technologies Used

- **Python**
- **pandas** - Data manipulation and analysis
- **matplotlib** - Data visualization
- **plotly** - Interactive charts
- **Jupyter Notebook/Google Colab**

---

*This is a practice project focused on developing data analysis skills with pandas and visualization libraries.*
*Important note: some charts aren't showing in the notebook so it's better to run it to explore them.*

