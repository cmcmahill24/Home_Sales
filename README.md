# Home_Sales
Module 22 Challenge

My final version of code is labeled home_sales.ipynb. Resources: ChatGPT for overall coding and debugging issues. Background: In this challenge, you'll use your knowledge of SparkSQL to determine key metrics about home sales data. Then you'll use Spark to create temporary views, partition the data, cache and uncache a temporary table, and verify that the table has been uncached. Data retrieved from: "https://2u-data-curriculum-team.s3.amazonaws.com/dataviz-classroom/v1.2/22-big-data/home_sales_revised.csv"

## Findings: 
### Performance Comparison
- **Uncached Query Runtime**: 1.40 seconds  
- **Cached Query Runtime**: 0.51 seconds  
- **Parquet Query Runtime**: 0.64 seconds  

The cached query showed significant improvement over the uncached query. The Parquet query also performed efficiently due to its optimized storage format but was slightly slower than the cached query.

### Key Results
1. The average price of a four-bedroom house sold by year:
   - 2019: $300,263.70

   - 2020: $298,353.78

   - 2021: $301,819.44

   - 2022: $296,363.88

2. Homes with 3 bedrooms and 3 bathrooms have consistent pricing trends, with slight variation year-over-year.

3. Homes with higher "view" ratings generally have significantly higher average prices, indicating a correlation between views and property value.
