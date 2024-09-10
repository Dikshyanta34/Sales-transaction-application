##Sales Transaction Application ##
This is a database that any store can use where it allows to track their customer, product and all items sold to a customer and generate an invoice (bill). 

1. Create at least following tables: 
Product	 
Customer  
Sales Transaction 
Invoice 
Note: Each table must have primary key, Unique key and should have foreign key constraints (can have check constraints) 

2.Based on created tables, create the following using TSQL 

3. Store Procedures: 

a.Insert Product, Update Product, Select Product (Json as parameter for all SP preferred)  
b.Insert Customer, Update Customer, Select Customer 
c.Insert Sales Transaction, Update Sales Transaction, Select Sales Transaction 
d.Create Invoice with following conditions: 
i.)It should generate invoice and insert into Invoice table and each invoice generated should be tagged back to the related transaction. 
ii.)Number of invoices inserted should create only one invoice per customer. (a customer may buy 5 items but it should only generate one invoice (bill)) 
iii.)Should calculate discount of 5% for items whose total amount is less than or equal 500 and 10% if total amount is greater than 500. 

4. Script to insert 50 random information in all tables. Should use the insert SP. 

5. The primary key in all tables should start from 100.  

6. Query to return following:  
a.Whose name start with the letter "A" or ends with the letter "S" but should have the letter "K". 
b.Do not have any invoice yet.	 
c.Average number of products bought on current date. 
d.The customer who has spent highest amount in specific date rage. 
e.The product should have an expiry date. Delete a product that was never bought and was expired a week ago. 
f.Delete a product that was never bought and is about to expire in a week.  
g.Product should have a quantity column which shows the quantity of a product and a remaining column which should the remaining quantity of the product. This should be updated on the basis of transaction.    
h.Get the product of the year (The max quantity of a product bought this year.)  

7.  Function with following: 
Parameters:	 
a.Customer (can pass multiple ids e.g.: 103,904) 
b.Start Date and End date 
c.Entity (transaction or invoice)

Requirement: 
a.Should return sum of amount of the provided customers.  
b.Should return data having entered date in the date range provided. 

8. Store Procedure: 
Parameters: 
a.Start Date and End date 
b.Customer (if no customer Id passed then return all data else the given customers data only)

Requirement: 
a.Should have all the customers whose id and their information who were created within the date range 
b.Count of transactions made by all the customers 
c. Total Billed amount of customers 
d.Top product bought by the customer. (if a customer has bought 5 notebook,2 pencils and 1 bag then Notebook is the top product) 
Json used for parameter and to return values mandatory. 

 

 

 



 

 

 
