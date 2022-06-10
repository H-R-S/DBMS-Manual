## [Lab: 09]()
### Exercise
Question No. 1
We have the following tables which creates statement are
1.	create table supplier(S_NO int identity(1,1), SUP_ID varchar(50) primary key,SUP_NAME varchar (50), SUP_ADD varchar (50), SUP_NIC int, rank int)
2.	create table Product(Prod_ID varchar(50) primary key,Prod_Name varchar(50),[Price/Unit] float)
3.	create table Orders(Ord_ID varchar(50) primary key,Prod_ID varchar(50),Qty int,Totalrate int,SUP_ID varchar (50))

Write the Queries using Joins on above tables
1.	List of all supplier that palced order
2.	List of all Product that are supplied by supplier whose id is 101
3.	Find all order(s) of product named Rice
#### Query:
```
CREATE DATABASE Lab_9

CREATE TABLE Supplier (
	S_NO INT(10), 
	SUP_ID VARCHAR(50) PRIMARY KEY,
	SUP_NAME VARCHAR (50), 
	SUP_ADD VARCHAR (50), 
	SUP_NIC INT(10), 
	RANK INT(10)
);

INSERT INTO Supplier (S_NO, SUP_ID, SUP_NAME, SUP_ADD, SUP_NIC, RANK)
VALUES (1, 101, 'John', 'Street 69, London', 0123456789, 9),
       (2, 102, 'Alex', '14 Street, Scotland', 3456789012, 8),
       (3, 103, 'Parker', 'L Street, London', 0237864591, 10),
       (4, 104, 'Pele', 'Downtown, London', 9234567810, 8);
       
CREATE TABLE Product (
	Prod_ID VARCHAR(50) NOT NULL PRIMARY KEY,
	Prod_Name VARCHAR(50),
	Price_per_Unit FLOAT
);

INSERT INTO Product (Prod_ID, Prod_Name, Price_per_Unit)
VALUE ('Prod_1', 'Meat', 999.99),
      ('Prod_2', 'Rice', 599.99),
      ('Prod_3', 'Mix Fruits', 399.90),
      ('Prod_4', 'Mix Vegitables', 449.99);
      
CREATE TABLE Orders (
	Ord_ID VARCHAR(50) NOT NULL PRIMARY KEY,
	Prod_ID VARCHAR(50) REFERENCES Product(Prod_ID),
	Qty INT,
	Totalrate INT,
	SUP_ID VARCHAR(50) REFERENCES Supplier(SUP_ID)
);

INSERT INTO Orders (Ord_ID, Prod_ID, Qty, Totalrate, SUP_ID)
VALUES ('Ord_01', 'Prod_1', 3, 2999.97, 101),
       ('Ord_02', 'Prod_2', 5, 2999.95, 104),
       ('Ord_03', 'Prod_3', 2, 799.8, 102),
       ('ord_04', 'Prod_4', 8, 3999.92, 103);
       
SELECT Supplier.S_NO, Supplier.SUP_NAME, Supplier.SUP_ADD, Supplier.SUP_NIC,
Orders.Ord_ID, Orders.Prod_ID, Orders.Qty, Orders.Totalrate FROM Supplier
INNER JOIN Orders ON Supplier.SUP_ID = Orders.SUP_ID;

SELECT Orders.Prod_ID, Supplier.SUP_ID, Supplier.SUP_NAME FROM Orders
INNER JOIN Supplier ON Orders.SUP_ID = Supplier.SUP_ID
WHERE Supplier.SUP_ID LIKE 101;

SELECT Orders.Ord_ID, Orders.Prod_ID, Orders.Qty, Orders.Totalrate, Product.Prod_ID,
Product.Prod_Name, Product.Price_per_Unit FROM Orders
INNER JOIN Product ON Orders.Prod_ID = Product.Prod_ID
WHERE Prod_Name = 'Rice';
```
### Output ScreenShots:
#### Question: 01
![Q1](https://github.com/H-R-S/DBMS-Manual/blob/main/Lab_09/ScreenShots/q1.PNG)
#### Question: 02
![Q2](https://github.com/H-R-S/DBMS-Manual/blob/main/Lab_09/ScreenShots/q2.PNG)
#### Question: 03
![Q3](https://github.com/H-R-S/DBMS-Manual/blob/main/Lab_09/ScreenShots/q3.PNG)