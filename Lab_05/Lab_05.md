## [Lab: 05]()
### Exercise
Consider the following schema:
1.	Customer (cust_id, cust_name).
2.	Product (prod_code ,prod_name, unit_price)
3.	Customer_Order (order_code, order_date, cust_id)
4.	Order_Item (order_code, prod_code, num_of_units)

I.	Develop DDL of in SQL

II.	Add Column contact in Customer Table

III.Add Column company_name in Product Table

#### Query:
```
CREATE DATABASE Lab_05

CREATE TABLE Customer (
	Customer_id INT(10) NOT NULL,
	Customer_name CHAR(20),
	PRIMARY KEY (Customer_id)
);

CREATE TABLE Product (
	Product_code INT(10) NOT NULL,
	Product_name VARCHAR(20),
	Unit_price VARCHAR(10),
	PRIMARY KEY (Product_code)
);

CREATE TABLE Customer_Order (
	Order_code INT(10) NOT NULL,
	Order_date DATE NOT NULL,
	Customer_id INT(10) NOT NULL,
	PRIMARY KEY (Customer_id, Order_code)
);

CREATE TABLE Order_Item (
	Order_code INT(10) NOT NULL,
	Product_code INT(10) NOT NULL,
	Num_of_Units VARCHAR(20) NOT NULL,
	PRIMARY KEY (Order_code, Product_code)
);

ALTER TABLE Customer 
ADD Contact INT(11) NOT NULL;

ALTER TABLE Product
ADD Company_Name VARCHAR(20) NOT NULL;

```
### Output ScreenShots:
#### Customer Table:
![Customer Table](https://github.com/H-R-S/DBMS-Manual/blob/main/Lab_05/ScreenShots/customer_table.PNG)
#### Product Table:
![Product Table](https://github.com/H-R-S/DBMS-Manual/blob/main/Lab_05/ScreenShots/product_table.PNG)
#### Customer Order Table:
![Customer Order Table](https://github.com/H-R-S/DBMS-Manual/blob/main/Lab_05/ScreenShots/customer_order_table.PNG)
#### Order Item Table:
![Order Item Table](https://github.com/H-R-S/DBMS-Manual/blob/main/Lab_05/ScreenShots/order_item_table.PNG)
#### Add Column Contact in Customer Table:
![Add Column Contact in Customer Table](https://github.com/H-R-S/DBMS-Manual/blob/main/Lab_05/ScreenShots/add_column_contact_in_customer_table.PNG)
#### Add Column Company_Name in Product Table:
![Add Column Company_Name in Product Table](https://github.com/H-R-S/DBMS-Manual/blob/main/Lab_05/ScreenShots/add_column_company_name_in_product_table.PNG)