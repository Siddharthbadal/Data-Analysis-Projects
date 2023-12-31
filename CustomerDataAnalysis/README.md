# Customers Purchasing Data Analysis 

### Project Overview
This data analysis project aims to provide insights into the customers purchasing pattersns of an e-commerce company over the past few years. By analyzing various aspects of the customers data that include reviews, ratings, produtcs, we seek to identify trends, make data-driven recommendations, and gain a deeper understanding of the product's performance and overall sales patterns.

![chart](https://github.com/Siddharthbadal/Data-Analysis-Projects/assets/55015090/5c6660a1-4dd7-4c59-b880-0cf4e3b265ad)

  
### Database
Primary dataset of Customers was avilable on a csv file as well as a dqlite file. dataset containes multiple columns about products, time, reviws, rraing,and customer details.

### Python Libraries

  -  Pandas
  -  Matplotlib
  -  Seaborn
  -  Excel

### Data Cleaning and Preparation

Initial data preparation included folloing steps:
  -  Data loading and Data Inspection
  -  Handling missing and invalid records
  -  Data Formatting
  -  Adding new columns and segregating data on two main categories

### Data Analysis

EDA involved data exploration, sampling, adding and remvoing columns that help us to answer followig business trends:
- Top Selling Products
- Top Buyers
- Relationships between buying patterns and reviews and scores.
- Top reviews 
- Reviews sentiments analysis 
- Bar charts to understand the growth over time 

```python
        main_df = data.groupby(['UserId']).agg({
        'ProductId': 'count',
         'Summary':'count',
         'Text': 'count', 
         'Score': 'mean'}
    ).sort_values(by="ProductId", ascending=False)
```

![chart](https://github.com/Siddharthbadal/Data-Analysis-Projects/assets/55015090/3efcf4cf-029e-4e85-a441-eb09720fdd54)

### Findings
  - Found over 10 products which are frequently brought by customers.
  - Frequent buyers and non frequent buyers both have hihger postive ratings supported by sentiment analysis on reviews text.
  - Few Top selling products have higher five star ratings and four star ratings but not a specofic pattern across all products.
