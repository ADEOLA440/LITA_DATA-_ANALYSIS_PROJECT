# LITA_DATA_ANALYSIS_PROJECT

### Capstone-Project On Sales Transactions and Customer Subcription Dataset
[Project Overview For Sales Data   ](#Project-Overview_Sales_Data)

[Project Overview For Customer Subcription Data](#project-overview-for-customer-subcription-data) 

[Column Descriptions For Sales Data](#column-descriptions-for-sales-data)

[Column Descriptions For Customer Data](#column-descriptions-for-customer-data)

[Data Source](#data-source)

[Tools Used](#tools-used)  

[Data Cleaning and Preparations](#data-cleaning-and-preparations)  

[Exploratory Data Analysis For Sales Data](exploratory-data-analysis_for-sales-data) 

[Exploratory Data Analysis customer Data](exploratory-data-analysis-for-customer-data)

[Data Analysis](#data-analysis)  

[Data Visualization](#data-visualization) 

[My Result For Sales Data](#my-result-for-sales-data)  

[My Result For Customer Data](#my-result-for-customer-data)

### Project Overview For Sales Data 

It captures transactional sales data, providing a detailed view of customer orders, including product, region, and revenue information. It is ideal for analyzing sales trends, and regional performance, enabling insights into the drivers of revenue and high-demand products.

### Project Overview For Customer Subcription Data 

This dataset provides a comprehensive look at customer subscription patterns such as the subscription types and revenue, enabling insights into the drivers of pattern and high-demand subscription of different customer.

### Column Descriptions For Sales Data
-	OrderID: A unique identifier for each order.
-	CustomerId: A unique identifier for each customer.
-	Product: The specific product purchased in each transaction.
-	Region: The geographical location (e.g., North, South, East, West) where the order was placed.
-	OrderDate: The date when the order was made.
-	Quantity: The number of units purchased for each product in an order.
-	UnitPrice: The price per unit of the product.
-	Total Sales: The total sales value for the order, calculated as Quantity * UnitPrice

### Column Descriptions For Customer Data

-	CustomerID: Unique identifier for each customer.
-	CustomerName: Name of the customer (anonymized if necessary).
-	Region: Geographical area where the customer is located (e.g., North, South, East, West).
-	SubscriptionType: Type of subscription plan the customer is enrolled in (e.g., Basic, Premium).
-	SubscriptionStart: Start date of the customer's subscription.
-	SubscriptionEnd: End date of the customer's subscription.
-	Canceled: Indicates if the subscription was canceled (TRUE or FALSE).
-	Revenue: Revenue generated from the customer's subscription.
-	Subscription Duration: Duration (in days) of the subscription period

### Data Source:  
The main data sources for this analysis are the "Data Sales.csv" and "Customer.csv" files, which are open-source datasets available for free download from online repositories like Kaggle, FRED, or other similar platforms.

### Tools Used 
-Excel: Employed for data cleaning and visualization.

-SQL: Utilized for data cleaning through queries.

-Power BI: Used for both data cleaning and visualization.

### Data Cleaning and Preparations 
In the intial phase of Data Cleaning and Preparations, we perform the following action;
- Data loading and Inspection
- Handling missing variables
- Data Cleaning and Formatting 

#### Exploratory Data Analysis For Sales Data ON SQL
the exploratory of the Data to answer some questions about the data such as;
1. Retrieve the total sales for each product category.
2. Find the number of sales transactions in each region.
3. Find the highest-selling product by total sales value.
4. Calculate total revenue per product.
5. Calculate monthly sales totals for the current year.
6. Find the top 5 customers by total purchase amount.
7. Calculate the percentage of total sales contributed by each region.
8. Identify products with no sales in the last quarter.
Examples:
![SalesData SQL](https://github.com/ADEOLA440/LITA_DATA-_ANALYSIS_PROJECT/blob/main/SQL_SALESDATA.png)
![SalesDataSQL](https://github.com/ADEOLA440/LITA_DATA-_ANALYSIS_PROJECT/blob/main/Sales%20Data%20Sql.png)

#### Exploratory Data Analysis For Customer Data
the exploratory of the Data to answer some questions about the data such as;
1. Retrieve the total number of customers from each region.
2. Find the most popular subscription type by the number of customers.
3. Find customers who canceled their subscription within 6 months.
4. Calculate the average subscription duration for all customers.
5. Find customers with subscriptions longer than 12 months.
6. Calculate total revenue by subscription type.
7. Find the top 3 regions by subscription cancellations.
8. Find the total number of active and canceled subscriptions.
Examples
![CustomerData on SQL](https://github.com/ADEOLA440/LITA_DATA-_ANALYSIS_PROJECT/blob/main/SQL%20on%20CustomerData.png)
![CustomerData on SQL](https://github.com/ADEOLA440/LITA_DATA-_ANALYSIS_PROJECT/blob/main/Customerdata%20sql.png)

### Data Analysis 
This is where we include some basic lines of code or queries or even some of the DAX expressions used during my analysis; 

```SQL
select *
From Table Name = SalesData
```
```SQL
select *
From Table Name = CustomerData
```
### Data Visualization
![Sales Data](https://github.com/ADEOLA440/LITA_DATA-_ANALYSIS_PROJECT/blob/main/SalesData%20Pivot%20Table.png)
![Sales Data Visulisation](https://github.com/ADEOLA440/LITA_DATA-_ANALYSIS_PROJECT/blob/main/Data%20Visualisation%20on%20Salesdata.png)
![Customer Data](https://github.com/ADEOLA440/LITA_DATA-_ANALYSIS_PROJECT/blob/main/Customer%20Data%20Pivot%20Table.png)
![Customer Data Visualisation](https://github.com/ADEOLA440/LITA_DATA-_ANALYSIS_PROJECT/blob/main/Data%20Visalisation%20on%20CustomerData.png)


#### My Result For Sales Data 
Our Sales Data analysis tells a story of what the customers love and how they shop. Shoes are the star of sales, selling over 600,000 units and becoming the best-selling product. Meanwhile, socks, though popular, came in last.
Each month brought its own pattern,as the year went on, the first and second quarters showed strong, high sales. But as summer turned into fall, sales began to drop, and by the fourth quarter, they were down.
Looking at different regions, the South led the way,followed by the East, the North, and finally, the West. Each area added its own flavor to our overall numbers, but together, they showed the store’s success across the map.
the average sales rate was an impressive 211.78%, showing strong customer interest throughout the year.

#### My Result For Customer Data
Our Customer data analysis uncovered some interesting patterns in how our customers use their subscriptions. With a variety of plans available, the "Basic" subscription emerged as the most popular, accounting for over 50% of all subscriptions. It seems that simplicity and affordability have won over a large part of our customer base.
In terms of commitment, our subscribers have an average subscription duration of 365 days,as they renew their plans for a full year on average.
One region, however, stands out: the East. Unlike other regions, where some customers occasionally cancel their plans, the East shows a remarkable commitment to their subscriptions, with zero cancellations on record. This region’s loyalty adds a unique dynamic to our customer insights.
Lastly, the total revenue generated from all subscriptions reached an impressive 68 million. This figure reflects both the loyalty and the value our customers place on their subscriptions, building a strong financial foundation for our service.




























