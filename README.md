# Home_Sales_SparkSQL
## Introduction
- Use SparkSQL to read in home_sales data and determine the key metrics, create temporary views, partition the data, cache and uncache a temporary table and verify the table cache status.
## Findings
1. What is the average price for a four bedroom house sold per year, rounded to two decimal places?
 ![image](https://github.com/user-attachments/assets/668bce46-820d-433a-ad30-075ab950b621)
- The average price for a 4 bedroom house fluctuates slightly from year to year. There is no siginificant trend. The price decreased in 2020 and rose again in 2021. In 2022, the price was back to the price level in 2020.

2. What is the average price of a home for each year the home was built that have 3 bedrooms and 3 bathrooms, rounded to two decimal places?
 ![image](https://github.com/user-attachments/assets/c06bab62-a3e4-4390-a60e-a4fc6d2019f1)
- From 2010 to 2017, the price for a 3b3b house doesn't change a lot. The price range remains around $290,000.

3. What is the average price of a home for each year the home was built, that have 3 bedrooms, 3 bathrooms, with two floors, and are greater than or equal to 2,000 square feet, rounded to two decimal places?
 ![image](https://github.com/user-attachments/assets/fb190e06-4719-46be-858a-6136694baaf6)
- From 2010 to 2017, the price of a 3b3b&2F house remained relatively stable. In contrast, the price of 3b3b houses experienced more fluctuation, though no clear trend was evident.

4. The run-time comparison:
- Original data
 ![image](https://github.com/user-attachments/assets/d51b5bc0-cb97-4384-b50c-6677ed530734)

- Cache data
 ![image](https://github.com/user-attachments/assets/1bb5d78e-31ef-4419-98af-543bc2b4270f)

- Parquet data
  ![image](https://github.com/user-attachments/assets/e9abbc67-77d8-42f7-9881-7ac086474ef0)

- It's obvious that Cache data and Parquet data experience faster runtime than the original data does. It is because of the properties and benefits of cahcing and parquet data format. When query the cached data, it can be retrieved directly from memory and is not needed to be read from disk. Parquet is a columnar storage format specifically designed for efficient data processing.


  
 
