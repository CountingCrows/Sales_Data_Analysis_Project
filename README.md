# Sales_Data_Analysis_Project
This project is a set of real world data science practice from merging the data, data cleaning, EDA, to data visualization using python. We are going to analyze and answer business questions about 12 months worth of sales data. The data contains hundreds of thousands of electronics store purchases broken down by month, product type, cost, purchase address, etc.

## Dataset
This dataset is collected from https://github.com/KeithGalli/Pandas-Data-Science-Tasks/tree/master/SalesAnalysis/Sales_Data. The dataset is consisted of 12 months of sales data of a store in the U.S. 

## Tasks
- Merging 12 months of seperated data
- Drop NaN values from DataFrame
- Removing rows based on a condition
- Change the type of columns (to_numeric, to_datetime, astype)

## Questions
- What was the best month for sales? How much was earned that month?
- What city sold the most product?
- What time should we display advertisemens to maximize the likelihood of customer’s buying product?
- What products are most often sold together?
- What product sold the most? Why do you think it sold the most?

## Other tasks include:
- Concatenating multiple csvs together to create a new DataFrame (pd.concat)
- Adding columns
- Parsing cells as strings to make new columns (.str)
- Using the .apply() method
- Using groupby to perform aggregate analysis
- Plotting bar charts and lines graphs to visualize our results
- Labeling our graphs

## Results
- We find that the best month for sales is in December with an amount around $4.6 million.
- The city that sold the most products is San Fransisco (CA).
- We should display advertisements to maximize the likelihood of customer's buying products around 11 am and 7 pm.
- The products that are often sold together is an Iphone and a Lightning Charging Cable for an amount of 1005 transactions.
- The product that is sold the most is AA batteries (4 pack) for almost 30.000 orders and AAA batteries (4 pack) for more than 30.000 orders. This is due technologies in 2010's still depend on batteries and it's cheap price.
