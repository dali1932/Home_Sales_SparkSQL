# Home_Sales_SparkSQL
## Introduction
- Use SparkSQL to read in home_sales data and determine the key metrics, create temporary views, partition the data, cache and uncache a temporary table and verify the table cache status.
## Findings
1. What is the average price for a four bedroom house sold per year, rounded to two decimal places?
![image](https://github.com/user-attachments/assets/668bce46-820d-433a-ad30-075ab950b621)
The average price for a 4 bedroom house fluctuates slightly from year to year. There is no siginificant trend. The price decreased in 2020 and rose again in 2021. In 2022, the price was back to the price level in 2020.

3. What is the average price of a home for each year the home was built that have 3 bedrooms and 3 bathrooms, rounded to two decimal places?
![image](https://github.com/user-attachments/assets/c06bab62-a3e4-4390-a60e-a4fc6d2019f1)
From 2010 to 2017, the price for a 3b3b house doesn't change a lot. The price range remains around $290,000.

4. What is the average price of a home for each year the home was built, that have 3 bedrooms, 3 bathrooms, with two floors, and are greater than or equal to 2,000 square feet, rounded to two decimal places?
![image](https://github.com/user-attachments/assets/fb190e06-4719-46be-858a-6136694baaf6)
From 2010 to 2017, the price of a 3b3b&2F house remained relatively stable. In contrast, the price of 3b3b houses experienced more fluctuation, though no clear trend was evident.

  
 
