# Vrinda Store Data Analysis

## Summary
This project analyzes the sales performance of Vrinda Store for the year 2022 using Excel. The dataset consists of 31,047 rows and includes key customer and order details such as Order ID, Gender, Age, Age Group, Date, Month, Status, Channel, Category, Qty, Amount, and Shipping details.\
\
The objective of this analysis is to help Vrinda Store understand customer behavior, sales trends, and top-performing channels in order to design strategies for increasing sales in 2023.



## Obectives
Vrinda store wants to create an annual sales report for 2022.\
So that, Vreinda can understand their customers and grow more sales in 2023.


## Questions to solve
1: Compare the sales and orders using single chart.\
2: Which month got the highest sales and orders?\
3: Who purchased more Men or Womenin 2022?\
4: What are different order status in 2022?\
5: List top states contributing to the sales?\
6: Relation between age and gender based on number of orders.\
7: Which channel is contributing to maximum sales?\
8: Higest selling category?


### 1 Data Cleaning
Checkes in all the colunms Null values and thier Data types to ensure Date, Numberic and String are in correct form./
In Gender colunm thier two categories Man and Woman but some where written as M instead of Man and written W instead of Woman So in that case I replace M with Man and M with Woman.\
In Quantity colunm also written one and two instead of 1 and 2. So, I also replaced one and two with 1 and 2.


### 2 Data Processing

### Age colunm
In Age colunm thier We can make a relationship because they have a lot of numbers.\
So in this case, I make a Group Age colunm to make groups of age to easy to apple relationship.
Used IF() formula to apply conditionof  groups. The formaula is:\
<code><B>=IF(E2>=50,"Senior",IF(E2>=30<"Adult",Teenager"))</B></code>\
Used grouped if the ages is greater tahn or equal to 50 will come in Senior category.\
If the grouped ages is greater than or equal to 30 and less than 50 will come in Adult category.\
And the remain which is greater than or equal to 18 and less than 30 will be come in Teenager category.\
In this way it's easy to creates the relationships between them.

### Date colunm
From the Date colunm, I was need Months for creating relationships.\
I used TEXT() formula to separate months from date. The formula is:\
<code><B>=TEXT(G2,"mmm")</B></code>\
G2 is nothing but Date colunm name in Excel, and triple m is nothing but give you three leters months name (like Jan, Feb etc.) using TEXT() formula in Excel.


### 3 Data Analyzing
Created PivotTables For Each of the above questions and created a PivotChart.\
Created attractive and readable with cahrt Title and make Relationship with all charts by using Insert Slicer function by Month, Channel, and Category colunms, give me a readable and attractive report that get insights and to increase sales in coming year 2023. 


## Key Insights
Sales vs Orders: Strong positive correlation – higher orders drive higher sales.\
Top Month: March recorded the highest sales and orders.\
Customer Profile: Women (~65%) purchased more than men.\
Order Status: Majority orders were delivered, with smaller portions in returned/cancelled.\
Top States: Maharashtra, Karnataka, and Uttar Pradesh contributed ~35% of total sales.\
Age & Gender: Adults (30–49 years) contributed the most (~50%), with women leading.\
Sales Channels: Amazon, Flipkart, and Myntra drove ~80% of sales.\
Top Category: Apparel was the highest-selling product category.


## Final Conclusion to Improve Vrinda Store Sales:
Vrinda Store should focus marketing efforts on women aged 30–49 in Maharashtra, Karnataka, and Uttar Pradesh, with promotions on Amazon, Flipkart, and Myntra. Targeted ads, discount campaigns, and loyalty offers in these segments can significantly boost sales in 2023.
