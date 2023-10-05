![image](https://github.com/CountingCrows/Sales_Data_Analysis_Project/assets/85608120/8b6be000-dd85-430d-b148-715b309127a0)# Sales_Data_Analysis_Project
This project is a set of real world data science practice from merging the data, data cleaning, EDA, to data visualization using python. We are going to analyze and answer business questions about 12 months worth of sales data. The data contains hundreds of thousands of electronics store purchases broken down by month, product type, cost, purchase address, etc.

## Dataset
This dataset is collected from https://github.com/KeithGalli/Pandas-Data-Science-Tasks/tree/master/SalesAnalysis/Sales_Data. The dataset is consisted of 12 months of sales data of a store in the U.S. 

## Data Preparation 
The dataset contains 12 seperate csv files from January 2019 to December 2019. Before analyzing and cleaning the data, we merge the 12 seperate datasets into 1 scv file by doing this command:

![image](https://github.com/CountingCrows/Sales_Data_Analysis_Project/assets/85608120/e299c8d3-ceda-4e22-afa1-9daa8be7229a)

## Data Cleaning
For the data cleaning proses, first we drop all rows containing NaN values. 

![image](https://github.com/CountingCrows/Sales_Data_Analysis_Project/assets/85608120/8a166669-277f-4c7d-94d3-4ccfb17cad72)

We can see that the "Order Date" column has the date and time of the purchase, so we want to seperate the values into a new column. So, for the data cleaning process, other several tasks done are:
  - Find "Or" and delete it
  - Convert columns to the correct type

  - ![image](https://github.com/CountingCrows/Sales_Data_Analysis_Project/assets/85608120/5908fb73-059b-4cc1-a918-7f322150a696)

## Data Analysis
- We want to figure out what was the best month for sales? And How much was earned in that particular month?
We first make 2 additional columns, a "Month" column that contains the value of the month from the "Order Date" column. Also, we add a "Sales" column by multiplying the "Quantity Order" column and "Price Each" column.

![image](https://github.com/CountingCrows/Sales_Data_Analysis_Project/assets/85608120/c0c146ef-8c55-4ce4-a2fb-2448aab08b01)

Then, we add a "City" column extracting the city values from the "Purchase Address" column. We execute this command using the .apply() method.

![image](https://github.com/CountingCrows/Sales_Data_Analysis_Project/assets/85608120/44bef7cd-0917-4b76-82ab-7317cb9fc976)

![image](https://github.com/CountingCrows/Sales_Data_Analysis_Project/assets/85608120/e1cc0217-8378-45d7-b72c-ae38e530988b)

From here, we can easily examine the best month for sales and how much was earned from January 2019 to December 2019. 

![image](https://github.com/CountingCrows/Sales_Data_Analysis_Project/assets/85608120/b8ef71eb-0016-4bfb-88a4-8b4a5b6293f5)

![image](https://github.com/CountingCrows/Sales_Data_Analysis_Project/assets/85608120/b81e278f-cd7b-409b-9b66-0d1ece0f65af)

The highest sales in the US of this store was in December with more than $4 million sales.

- What city sold the most product?

![image](https://github.com/CountingCrows/Sales_Data_Analysis_Project/assets/85608120/7855b2e0-a83e-4b6c-a948-70620a56d82e)

![image](https://github.com/CountingCrows/Sales_Data_Analysis_Project/assets/85608120/c9c7e83f-7289-43fa-901b-abb36db440e8)

The city that contributed the highest sales in the U.S. San Francisco(CA) for above $8 million.

- What time should we display advertisemens to maximize the likelihood of customer’s buying product?


- What products are most often sold together?


- What product sold the most? Why do you think it sold the most?


## Results
- We find that the best month for sales is in December with an amount around $4.6 million.
- The city that sold the most products is San Fransisco (CA).
- We should display advertisements to maximize the likelihood of customer's buying products around 11 am and 7 pm.
- The products that are often sold together is an Iphone and a Lightning Charging Cable for an amount of 1005 transactions.
- The product that is sold the most is AA batteries (4 pack) for almost 30.000 orders and AAA batteries (4 pack) for more than 30.000 orders. This is due technologies in 2010's still depend on batteries and it's cheap price.
