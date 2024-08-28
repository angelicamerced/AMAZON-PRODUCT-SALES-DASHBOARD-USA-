# Amazon-Product-Sales-Dashbaord-USA-

### Situation
Amazon, one of the largest online retailers in the USA, offers an extensive catalog of over 12 million products. Despite this vast inventory, there was a need for a comprehensive analysis to understand key aspects of product performance and sales trends. The company wanted to gain insights into which products achieved the highest sales, the optimal pricing strategies for different product categories and how discounts affected sales performance.

### Task 
The task was to perform a detailed analysis of the Amazon sales dataset, which consists of 1.43 million products, in order to extract actionable insights for optimizing sales and product performance.

The goal was to create a Power BI report that presents the key metrics and KPIs for sales, product performance and highlight the best-selling items.

### Action
Data Sources: https://www.kaggle.com/datasets/asaniczka/amazon-products-dataset-2023-1-4m-products

Data Collection and Preparation: Extracted data from different CSV format files, which consisted of:
- amazon_categories
- amazon_products
  
Cleaned and preprocessed the data to handle missing values, remove duplicates, remove unnecessary columns and standardize formats, ensuring accuracy and consistency for analysis using Power Query. 

Added is_valid column to amazon_products to display a True or False based on if the price is greater than the list_price and list_price is not equal to 0, then filtered out rows with TRUE values and changed the type of is_valid column to Boolean.

Added discount_price column to amazon_products based on this formula -> if list_price is not equal to 0 then list_price minus price else 0.

Added discount_percentage column and rounded up the numbers.

Data Modeling: Established relationships between tables:
- `amazon_products` (`category_id`) linked to `amazon_categories` (`id`)

Metrics and KPIs: Defined and calculated key performance indicators (KPIs) such as Original Revenue, Discounted Revenue, Quantity Sold, Average Price, Average Ratings, Best Seller Products 

Report Design: Developed a Power BI report featuring interactive dashboards with visualizations like bar charts to show sales performance across different dimensions. 

### Result
![amazon dashboard](https://github.com/angelicamerced/Amazon-Product-Sales-Dashboard-USA-/blob/main/amazon.jpg)

The revenue from discounted products, totaling $4.65 billion, surpasses the revenue from products sold at their original prices, which amounts to $2.7 billion, by approximately 72.2%. 

﻿At 483, Sports & Fitness had the highest Best Seller Count and was 86.49% higher than Sports & Outdoors, which had the lowest Best Seller Count at 259.﻿﻿

The leading revenue contributors are the PlayStation 5 and Xbox Series X consoles, which together account for a substantial portion of total sales, exceeding $9.9 million.

Girls' Clothing accounted for 14.18% of Number of Products.﻿﻿


﻿﻿



