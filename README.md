Sales Analysis Project - Lebanon & Jordan
A mini data analysis project focused on practicing pandas data preprocessing and data visualization using matplotlib and plotly. This project analyzes sales data from a business operating both online and offline in Lebanon and Jordan.
📊 Project Overview
This project demonstrates essential data analysis skills including:

Data cleaning and preprocessing with pandas
Exploratory data analysis (EDA)
Creating meaningful visualizations
Extracting business insights from sales data

📋 Dataset
The dataset contains sales records with the following columns:

order_id: Unique identifier for each order
customer_id: Customer identifier
units_sold: Number of units sold
unit_prices_usd: Price per unit in USD
salesman: Sales representative
total_amount: Total order value
commission: Commission earned
sector: Business sector/category
channel: Sales channel (online/offline)

Geographic Coverage: Lebanon and Jordan
Sales Channels: Online and Offline
🎯 Analysis Focus Areas
Data Preprocessing

Data cleaning and validation
Handling missing values
Data type conversions
Feature engineering

Business Insights

Sales performance by country (Lebanon vs Jordan)
Online vs Offline channel analysis
Year-over-Year growth trends
Salesman performance analysis
Sector-wise sales distribution
Commission analysis

Visualizations

Annual sales trends by country
Channel performance comparisons
Sales distribution across sectors
Top performing salespeople
Geographic sales heatmaps

🛠️ Technologies Used

Python 3.x
pandas - Data manipulation and analysis
matplotlib - Static data visualizations
plotly - Interactive visualizations
numpy - Numerical computations
Jupyter Notebook/Google Colab - Development environment

🚀 Getting Started
Prerequisites
bashpip install pandas matplotlib plotly numpy jupyter
Installation

Clone the repository:

bashgit clone https://github.com/yourusername/sales-analysis-lebanon-jordan.git
cd sales-analysis-lebanon-jordan

Install required packages:

bashpip install -r requirements.txt

Launch Jupyter Notebook:

bashjupyter notebook
Or open the Google Colab notebook directly: Sales Analysis Notebook
📁 Project Structure
sales-analysis-lebanon-jordan/
│
├── data/
│   └── sales_data.csv          # Raw sales data
│
├── notebooks/
│   └── sales_analysis.ipynb    # Main analysis notebook
│
├── visualizations/
│   ├── annual_trends.png       # Sales trends charts
│   ├── channel_comparison.png  # Online vs Offline analysis
│   └── geographic_analysis.png # Country-wise performance
│
├── README.md
└── requirements.txt
📈 Key Findings
[Add your main insights here after completing the analysis]

Annual sales growth trends between Lebanon and Jordan
Performance comparison of online vs offline channels
Top performing sectors and sales representatives
Seasonal patterns in sales data

🔍 Sample Code
Data Preprocessing
python# Convert year to integer for proper plotting
df['year'] = df['year'].astype(int)

# Group sales by year and country
annual_sales_country = df.groupby(['year', 'country_code'])['total_amount'].sum().unstack()

# Calculate Year-over-Year percentage change
yoy_change = annual_sales_country.pct_change(axis=0) * 100
Visualization Example
pythonimport matplotlib.pyplot as plt

plt.figure(figsize=(12, 6))
for country in annual_sales_country.columns:
    plt.plot(annual_sales_country.index, annual_sales_country[country], 
             marker='o', label=country)

plt.xlabel('Year')
plt.ylabel('Total Sales ($)')
plt.title('Annual Sales Trends by Country')
plt.xticks(annual_sales_country.index)  # Show only actual years
plt.legend()
plt.grid(True)
plt.show()
🎓 Learning Objectives
This project helps practice:

Pandas operations: groupby, aggregations, data cleaning
Data visualization: matplotlib and plotly chart creation
Business analysis: extracting meaningful insights from data
Data storytelling: presenting findings effectively

🤝 Contributing
This is a learning project, but suggestions and improvements are welcome!

Fork the project
Create a feature branch (git checkout -b feature/improvement)
Commit your changes (git commit -m 'Add some improvement')
Push to the branch (git push origin feature/improvement)
Open a Pull Request

📄 License
This project is open source and available under the MIT License.
👤 Author
Your Name

GitHub: @yourusername
LinkedIn: Your LinkedIn

🙏 Acknowledgments

Data analysis techniques learned from various online resources
Inspiration from real-world business analytics challenges
Thanks to the pandas and matplotlib communities for excellent documentation


This project is part of my data analysis learning journey. Feedback and suggestions are always welcome!
