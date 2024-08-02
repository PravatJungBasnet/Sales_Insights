# Sales_Insights

# Sales_Insights


# Airlines-Dashboard

### Dashboard Link : https://app.powerbi.com/groups/me/reports/384d017e-e935-44dc-9e7d-1626c1a36de1/ReportSection

## Problem Statement

This dashboard helps the Sales_Insights understand their Company Sales better. It helps the Company know Customer Engagement.  It helps to anaysis the total revenue collected and to see revenue throuh different area. It also helps to find out top sales etc.




### Data Analyst using sql 

# Show all customer records

SELECT * FROM customers;

 #
 Show total number of customers

SELECT count(*) FROM customers;

# Show transactions for Chennai market (market code for chennai is Mark001

 SELECT * FROM transactions where market_code='Mark001';

# Show distrinct product codes that were sold in chennai

SELECT distinct product_code FROM transactions where market_code='Mark001';

# Show transactions where currency is US dollars

SELECT * from transactions where currency="USD"

# Show transactions in 2020 join by date table

SELECT transactions.*, date.* FROM transactions INNER JOIN date ON transactions.order_date=date.date where date.year=2020;

# Show total revenue in year 2020,

SELECT SUM(transactions.sales_amount) FROM transactions INNER JOIN date ON transactions.order_date=date.date where date.year=2020 and transactions.currency="INR\r" or transactions.currency="USD\r";

# Show total revenue in year 2020, January Month,

SELECT SUM(transactions.sales_amount) FROM transactions INNER JOIN date ON transactions.order_date=date.date where date.year=2020 and and date.month_name="January" and (transactions.currency="INR\r" or transactions.currency="USD\r");

# Show total revenue in year 2020 in Chennai

SELECT SUM(transactions.sales_amount) FROM transactions INNER JOIN date ON transactions.order_date=date.date where date.year=2020 and transactions.market_code="Mark001";


           
           
  
  
# In our dataset, Some parameters were assigned value 0 -, remove those data using filter in poer Bi





        


 
 

# Snapshot of Dashboard (Power BI Service)

![Alt text](https://raw.githubusercontent.com/PravatJungBasnet/Sales_Insights/main/Screenshot%202024-08-02%20141933.png
)




 
 # Report Snapshot (Power BI DESKTOP)

 



# Insights

A single page report was created on Power BI Desktop & it was then published to Power BI Service.

Following inferences can be drawn from the dashboard;

### [1] Total Number of Customers = 38

   Total Revenue  = 985M
   Total Sales quantity  = 2M


   
