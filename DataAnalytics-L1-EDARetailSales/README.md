# EDA on Retail Sales Data

**Intern:** Sanjeev Kumar Yadav
**Track:** Data Analytics, Oasis Infobyte (OIBSIP)
**Task:** Level 1, Task 1: EDA on Retail Sales Data

## Objective
Perform an Exploratory Data Analysis (EDA) on a retail sales dataset to uncover sales patterns, customer behaviour trends and actionable business insights.

## Dataset
- Retail Sales Dataset (Kaggle, by mohammadtalib786)
- 1,000 rows and 9 columns: Transaction ID, Date, Customer ID, Gender, Age, Product Category, Quantity, Price per Unit, Total Amount
- Date range: 1 Jan 2023 to 1 Jan 2024

## Tools Used
Python, pandas, numpy, matplotlib, seaborn, Jupyter Notebook (VS Code)

## What I Did
1. Data inspection: shape, data types, null values and duplicate check
2. Descriptive statistics: mean, median, mode and standard deviation
3. Time series analysis: monthly and quarterly sales trends
4. Customer demographics: age groups and gender breakdown
5. Product analysis: revenue and quantity by product category
6. Correlation heatmap of numerical variables
7. Extra insights: age group vs. category sales heatmap and gender-wise category preference

## Key Findings
- The dataset has 1,000 transactions with total sales of 456,000.
- The average transaction value is 456, but the median is only 135. A few high-value transactions pull the average up, so the data is right-skewed.
- Sales peaked in May 2023 (53,150), and Q4 2023 was the strongest quarter (126,190). Jan 2024 has only one day of data, so it was not treated as a real low month.
- Within Q4, November (34,920) was weaker than October (46,580) and December (44,690).
- Category revenue is close: Electronics 156,905, Clothing 155,580 and Beauty 143,515. Beauty is last, about 8.5% below Electronics.
- The 46-55 age group has the most transactions (229) and the highest sales (100,690).
- The 18-25 group has the fewest transactions (169) but the highest average spend per transaction (about 500). The 56-65 group has the lowest (about 412).
- Gender split is nearly even: Female 51% and Male 49%. Total spending: Female 232,840 and Male 223,160.
- Total Amount correlates more strongly with Price per Unit (0.85) than with Quantity (0.37), so sales are driven more by price than by quantity.

## Business Recommendations
1. **Push the Beauty category:** Its revenue is about 8.5% below Electronics. Bundle offers and discounts can help close the gap.
2. **Target age groups differently:** Reward the 46-55 group (largest revenue source) with loyalty offers, and run campaigns to attract more transactions from the 18-25 group, whose average spend is highest.
3. **Plan for seasonality:** Increase stock and marketing before May and Q4, and run festive offers in November, which was the weakest month of Q4.
4. **Use price-based strategy:** Since sales depend more on price than quantity, test premium products and different price tiers.

## Limitations
- The dataset has no product names or product IDs, so the "top 10 products" analysis was replaced with category-wise revenue and quantity analysis, plus the top 10 customers by spending.
- Jan 2024 contains only one day of data, so it was excluded from month-to-month comparisons.

## Screenshots
![Monthly Sales Trend](screenshots/monthly_trend.png)
![Revenue by Category](screenshots/category_revenue.png)
![Correlation Heatmap](screenshots/correlation_heatmap.png)

## How to Run
```
pip install pandas numpy matplotlib seaborn jupyter
jupyter notebook retail_sales_eda.ipynb
```

## Links
- GitHub: https://github.com/Sanjeevyadav9555/OIBSIP
