# Online-Retailer-in-UK

# UK Online Retail Data Analysis

## Overview

This project performs a comprehensive analysis of transactional data from a UK-based online retailer specializing in unique all-occasion gifts. The dataset contains transactions occurring between December 2010 and December 2011, with over 500,000 records capturing customer purchasing patterns, product performance and sales trends. The analysis explores customer behavior, revenue patterns and market segmentation to uncover actionable business insights for strategic decision-making.

## Features

**Data Cleaning**: Handles missing values, cancellations, negative quantities and outliers to prepare a robust dataset for analysis.

**Exploratory Data Analysis (EDA)**: Includes temporal analysis, customer segmentation and product performance evaluation to uncover purchasing patterns and seasonal trends.

**Feature Engineering**: Creates derived metrics such as total transaction value, customer lifetime value and purchase frequency for deeper insights.

**Customer Segmentation**: Applies RFM (Recency, Frequency, Monetary) analysis and clustering algorithms to identify distinct customer groups.

**Market Basket Analysis**: Identifies frequently purchased product combinations to inform cross-selling and bundling strategies.

**Visualizations**: Provides clear charts, heatmaps and geographic visualizations to illustrate sales patterns, customer distributions and revenue trends.

## Installation

### Prerequisites

- Python 3.x
- pip (Python package installer)
- Required libraries: `numpy`, `pandas`, `matplotlib`, `seaborn`, `scikit-learn`, `plotly`

### Steps

1. Clone the repository:
```bash
git clone https://github.com/NicholusMuthomi/Online-Retailer-in-UK
```

2. Navigate to the project directory:
```bash
cd Online-Retailer-in-UK
```

3. Install the required libraries:
```bash
pip install -r requirements.txt
```

4. Run the analysis notebook:
```bash
jupyter notebook UK_Online_Retail_Data_Analysis.ipynb
```

## Code Functionality

**Data Loading and Cleaning**: Imports the dataset, removes cancelled orders (invoices starting with 'C'), handles missing CustomerIDs and filters out erroneous records with negative quantities or prices.

**Feature Transformation**: Calculates total transaction amounts, extracts temporal features (month, day, hour) and aggregates customer-level metrics for segmentation.

**Exploratory Analysis**: Analyzes sales trends over time, identifies top-selling products, evaluates country-wise revenue contributions and examines customer purchase frequencies.

**Customer Segmentation**: Implements RFM analysis to score customers based on recency, frequency and monetary value. Groups customers using K-Means clustering to identify high-value, at-risk and dormant segments.

**Market Basket Analysis**: Applies association rule mining to discover product combinations frequently purchased together, supporting recommendation strategies.

**Visualizations**: Generates time series plots for sales trends, bar charts for top products and customers, geographic maps for regional analysis and heatmaps for correlation analysis.

## Results

### Key Insights

**Sales Trends**: Revenue peaks in November and December, indicating strong holiday season demand. Midweek purchases dominate, with Thursday showing the highest transaction volumes.

**Top Markets**: The United Kingdom accounts for the majority of sales, followed by Germany, France and EIRE. International markets represent significant growth opportunities.

**Product Performance**: White Hanging Heart T-Light Holder, Regency Cakestand 3 Tier and Jumbo Bag Red Retrospot are among the best-selling items by quantity.

**Customer Behavior**: A small percentage of customers (approximately 20%) contribute to the majority of revenue (80%), following the Pareto principle. Average order value and purchase frequency vary significantly across customer segments.

### Customer Segmentation

Customers were segmented into distinct groups based on RFM scores:

- **Champions**: High recency, frequency and monetary scores. These customers purchase frequently, recently and spend significantly.
- **Loyal Customers**: Moderate to high frequency with consistent monetary value.
- **At-Risk**: Previously valuable customers showing declining engagement.
- **Lost**: Customers with low recency scores who have not purchased in several months.

The K-Means algorithm with optimal cluster number (k=4) achieved a silhouette score of 0.58, indicating well-separated customer segments.

### Market Basket Analysis

Association rules revealed strong product affinities:

- Customers purchasing storage items frequently buy decorative products together.
- Gift sets and seasonal items show high co-purchase rates during holiday periods.
- Wholesale customers exhibit distinct purchasing patterns compared to retail buyers.

## Business Implications

**Marketing Strategy**: Target Champions and Loyal Customers with exclusive offers and early access to new products. Re-engage At-Risk customers through personalized campaigns.

**Inventory Management**: Stock up on top-selling products before peak seasons. Optimize inventory levels based on monthly demand patterns.

**Product Bundling**: Create product bundles based on association rules to increase average order value and improve customer satisfaction.

**Geographic Expansion**: Focus marketing efforts on high-performing international markets while exploring untapped regions.

**Customer Retention**: Implement loyalty programs for high-value segments and develop win-back campaigns for dormant customers.

## Contributing

Contributions are welcome! If you have suggestions for improvements or find any issues, please open an issue or submit a pull request.

## License

This project is licensed under the MIT License. See the LICENSE file for details.

## Contact

For inquiries or feedback, please reach out to:

**Email**: muthominicholus22@gmail.com

**GitHub**: [NicholusMuthomi](https://github.com/NicholusMuthomi)

---

## Dataset Information

The dataset used in this analysis is sourced from the UCI Machine Learning Repository. It contains transactional data from a UK-based non-store online retail company that primarily sells unique all-occasion gifts. Many customers are wholesalers.

**Attributes**:
- **InvoiceNo**: Invoice number (6-digit unique identifier; 'C' prefix indicates cancellation)
- **StockCode**: Product code (5-digit unique identifier)
- **Description**: Product name
- **Quantity**: Number of units per transaction
- **InvoiceDate**: Transaction date and time
- **UnitPrice**: Product price per unit (GBP)
- **CustomerID**: Unique customer identifier
- **Country**: Customer's country of residence

## Acknowledgments

Data provided by Dr. Daqing Chen, Director of the Public Analytics group, and made available through the UCI Machine Learning Repository.
