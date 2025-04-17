# Supermarket-Sales

## 1. Context
  The dataset used in this project is available on Kaggle and can be found by searching "Supermarket Sales" in the search bar. It contains historical sales records from a supermarket company, covering transactions from three different branches over a period of three months.

To enhance performance and minimize data redundancy, dimension tables—such as Location, Product, Time, and Customer—were extracted from the main fact table (supermarket_table). These were then used to construct a star schema model, linking the fact table with the derived dimensions.

Furthermore, DAX functions were utilized to create calculated columns and new measures for better data visualization and trend analysis.
The attribute information is detailed below.

- **Invoice id:** Computer generated sales slip invoice identification number
- **Branch:** Branch of supercenter (3 branches are available identified by A, B and C).
- **City:** Location of supercenters
- **Customer type:** Type of customers, recorded by Members for customers using member card and Normal for without member card.
- **Gender:** Gender type of customer
- **Product line:** General item categorization groups - Electronic accessories, Fashion accessories, Food and beverages, Health and beauty, Home and lifestyle, Sports and travel
- **Unit price:** Price of each product in $
- **Quantity:** Number of products purchased by customer
- **Tax:** 5% tax fee for customer buying
- **Total:** Total price including tax
- **Date:** Date of purchase (Record available from January 2019 to March 2019)
- **Time:** Purchase time (10am to 9pm)
- **Payment:** Payment used by customer for purchase (3 methods are available – Cash, Credit card and Ewallet)
- **COGS:** Cost of goods sold
- **Gross margin percentage:** Gross margin percentage
- **Gross income:** Gross income
- **Rating:** Customer stratification rating on their overall shopping experience (On a scale of 1 to 10)

  ## 2. Analysis
  ### 2.1 Sales Overview by City and Product Type

  ![image](https://github.com/user-attachments/assets/62b24ac7-f640-409d-a6eb-c116bf2e69a8)
  
﻿Naypyitaw had the highest total Sum of Cost of goods sold at 105,303.53, followed by Yangon at 101,143.21 and Mandalay at 101,140.64.﻿﻿
﻿﻿﻿﻿Food and beverages in City  made up 7.36% of Sum of Cost of goods sold.﻿﻿
﻿﻿Naypyitaw had the highest average Sum of Cost of goods sold at 17,550.59, followed by Yangon at 16,857.20 and Mandalay at 16,856.77.﻿﻿
﻿﻿The line chart displays the sum of quantity sold by month across various product types, showing a noticeable dip in February for all categories—particularly fashion accessories and sports and travel—before rebounding in March. The donut chart presents the percentage share of each product type sold, revealing a fairly balanced distribution. Food and beverages lead slightly with 17.28%, followed closely by electronic accessories (17.62%), sports and travel (16.7%), and fashion accessories (16.37%). This combination of visuals effectively highlights both temporal trends and proportional contributions of different product categories.

### 2.2 Gross Margin & Sales Performance Overview

![image](https://github.com/user-attachments/assets/a5cf5a5d-a871-49f3-bb73-39e933a69170)

The line and bar chart in the top left shows daily trends of gross margin percentage and cost of goods sold for January, broken down by city, highlighting fluctuations in profitability and expenses. The waterfall chart in the middle shows cumulative growth in gross income over Q1 of 2019, with a steady increase from January to March. The bar chart on the right tracks the count of gross margin entries, indicating data volume growth over the months.

On the bottom left, product-specific gross income comparisons are shown across three cities, revealing variations in revenue contribution by branch and product type. The data table in the center provides detailed entries of gross income and margin percentages by day, offering a granular view. On the right, a gauge chart summarizes key statistics such as average (15.38), minimum (0.51), and maximum (49.65) gross income.



﻿﻿
﻿﻿
﻿
