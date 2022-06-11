# Database Management System Manual (Solved)
## Index:
- ### [Lab-01](https://github.com/H-R-S/DBMS-Manual/blob/main/Lab_01/Lab_01.md)
- ### [Lab-02](https://github.com/H-R-S/DBMS-Manual/blob/main/Lab_02/Lab_02.md)
- ### [Lab-03](https://github.com/H-R-S/DBMS-Manual/blob/main/Lab_03/Lab_03.md)
- ### [Lab-04](https://github.com/H-R-S/DBMS-Manual/blob/main/Lab_04/Lab_04.md)
- ### [Lab-05](https://github.com/H-R-S/DBMS-Manual/blob/main/Lab_05/Lab_05.md)
- ### [Lab-06](https://github.com/H-R-S/DBMS-Manual/blob/main/Lab_06/Lab_06.md)
- ### [Lab-07](https://github.com/H-R-S/DBMS-Manual/blob/main/Lab_07/Lab_07.md)
- ### [Lab-08](https://github.com/H-R-S/DBMS-Manual/blob/main/Lab_08/Lab_08.md)
- ### [Lab-09](https://github.com/H-R-S/DBMS-Manual/blob/main/Lab_09/Lab_09.md)
- ### [Lab-10](https://github.com/H-R-S/DBMS-Manual/blob/main/Lab_10/Lab_10.md)
- ### [Lab-11](https://github.com/H-R-S/DBMS-Manual/blob/main/Lab_11/Lab_11.md)
- ### [Lab-12](https://github.com/H-R-S/DBMS-Manual/blob/main/Lab_12/Lab_12.md)

## DBMS-Manual WordFile (with ScreenShots) : [DBMS_Manual_Solved.docs]()

___
## [Lab-01](https://github.com/H-R-S/DBMS-Manual/blob/main/Lab_01/Lab_01.md)
Question: 01
What are the disadvantages of file processing system?

### Answer:
```
Disadvantages of File Processing System:

- Slow access time
Direct access of files is very difficult and one needs to know the entire
hierarchy of folders to get to a specific file. This involves a lot of time.

- Presence of redundant data 
The same data can be present in two or more files which takes up more disc
space.

- Inconsistent Data
Due to data redundancy, same data stored at different places might not match
to each other.

- Data Integrity Problems
The data present in the database should be consistent and correct. To achieve
this, the data should must satisfy certain constraints.

- Difficulty in recovery of corrupt data
Recovery or backup of lost and corrupt data is nearly impossible in case of File
Processing System.

- Lack of Atomicity
Operations performed in the database must be atomic i.e. either the operation
takes place as a whole or does not take place at all.

- Unauthorized Access
Anyone who gets access to the file can read or modify the data.
```
___
## [Lab-02](https://github.com/H-R-S/DBMS-Manual/blob/main/Lab_02/Lab_02.md)
### Question 1
Modern School of higher education has around 2000 students and three departments. The students belong to various departments in the school. Every department has a Head of Department along with teachers. The head of department manages his departmental teachers and the students belonging to his department. The head of department also teaches the students. All the head of departments report to the principal of the school. The principal manages the departments and also teaches the students. Handling the administrative staff of the school is also the responsibility of the principal. Every individual, except the students, are the employees of the school
Problem
●	Identify the entity
●	Identify the entity’s attribute
●	Identify the primary and foreign Keys
●	Identify relationship between Entities
●	Identify the Cardinality constraints
### Answer:
```
1. Entities:
Students
Departments
Head of Departments
Teachers
Principal
Administrative Staff

2. Entity Attributes:
Students (Student_ID, Name, Phone_no, Address)
Departments (Department_ID, Name, E-mail)
Head of Departments (Name, E-mail)
Teachers(Teacher_ID, Name, Phone_no, Experience)
Principal (Name, Phone_no)
Administrative Staff (Name, Phone_no)

3. Primary Key:
Student_Id
Department_ID
Teacher-ID

4. Relationship between Entities:
The relationship between Student and Department is Many to Many.
The relationship between the Department and Head of Department is Manyto Many.
The relationship between the Head of Department and Teachers is One to Many.
The relationship between the Head of Department and Students is One to Many.
The relationship between the Principal and Department is One to Many.
The relationship between Administrative Staff and Principal is One to One.

5. ERD:
```
![ERD](https://github.com/H-R-S/DBMS-Manual/blob/main/Lab_02/ScreenShots/q1.PNG)


### Question 2
1.	a professor teaches zero, one or many classes and a class is taught by one professor
2.	a course may generate zero, one or many classes and a class comes from one course
3.	a class is held in one room but a room has many classes
### Answer:
```
1. A professor teaches zero, one or many classes and a class is taught by one professor
```
![Q1](https://github.com/H-R-S/DBMS-Manual/blob/main/Lab_02/ScreenShots/q2_a.PNG)
```
2. A course may generate zero, one or many classes and a class comes from one course
```
![Q2](https://github.com/H-R-S/DBMS-Manual/blob/main/Lab_02/ScreenShots/q2_b.PNG)
```
3. A class is held in one room but a room has many classes
```
![Q3](https://github.com/H-R-S/DBMS-Manual/blob/main/Lab_02/ScreenShots/q2_c.PNG)
___
## [Lab-03](https://github.com/H-R-S/DBMS-Manual/blob/main/Lab_03/Lab_03.md)
### Question 1
Question 1
Modern School of higher education has around 2000 students and three departments. The students belong to various departments in the school. Every department has a Head of Department along with teachers. The head of department manages his departmental teachers and the students belonging to his department. The head of department also teaches the students. All the head of departments report to the Principal of the school. The Principal manages the departments and also teaches the students. Handling the administrative staff of the school is also the responsibility of the Principal. Every individual, except the students, are the employees of the school
●	Identify the entity
●	Identify the entity’s attribute
●	Identify the primary and foreign Keys
●	Identify relationship between Entities
●	Identify the Cardinality constraints 
●	Draw ERD
### Answer:
```
1. Entities:
• Students
• Departments
• Head of Departments
• Teachers
• Principal
• Administrative Staff

2. Entity Attributes:
• Students (Student_ID, Name, Phone_no, Address)
• Departments (Department_ID, Name, E-mail)
• Head of Departments (Name, E-mail)
• Teachers (Teacher_ID, Name, Phone_no, Experience)
• Principal (Name, Phone_no)
• Administrative Staff (Name, Phone_no)


3. Primary Key:
• Student_Id
• Department_ID
• Teacher-ID

4. Relationship between Entities:
• The relationship between Student and Department is Many to Many.
• The relationship between the Department and Head of Department is
Manyto Many.
• The relationship between the Head of Department and Teachers is One
toMany.
• The relationship between the Head of Department and Students is One
toMany.
• The relationship between the Principal and Department is One to Many.
• The relationship between Administrative Staff and Principal is One to One.

5. ERD:
```
![Q1]()

### Question 2
Question 2 
1.	an invoice is written by one sales rep but a sales rep writes many invoices
2.	a vendor sells many products but a product is bought from one vendor
3.	an invoice has one or many products and a product is found on zero, one or many invoices
●	Identify the entity
●	Identify the entity’s attribute
●	Identify the primary and foreign Keys
●	Identify relationship between Entities
●	Identify the Cardinality constraints
●	Draw ERD
### Answer:
```
1. Entities:
• Invoice
• Sales_rep
• Vendor
• Product

2. Entity Attributes:
• Invoice (Invoice_no, Invoice_Product_ID,Invoice_Product_Quantity,
Invoice_Date, Customer_Name, Customer_Address)
• Sales_rep (Sales_rep_ID, Sales_rep_Name, Sales_rep_Phone.no)
• Vendor (Vendor_ID, Name, Address, Phone.no)
• Product (Product_ID, Name, Sales_rep_ID, Vendor_ID)

3. Primary Key:
• Invoice_no
• Invoice_Product_ID
• Sales_rep_ID
• Vendor_ID
• Product_ID

Foreign Key:

• Sales_rep_ID
• Vendor_ID
• Product_ID


4. Relationship between Entities:
• The relationship between Invoice and Sales_rep is One to One.
• The relationship between Sales_rep and Invoices is One to Many.
• The relationship between Vendor and Products is One to Many.
• The relationship between Product and Vendor is One to One.
• The relationship between Invoice and Products is One to Many.
• The relationship between Product and Invoices is One to Many.

5. ERD:
```
![Q2]()
___
## [Lab: 04]()
CASE - STUDY -II
The Prescriptions-R-X chain of pharmacies has offered to give you a free lifetime supply of medicine if you design its database. Given the rising cost of health care, you agree. Here’s the information that you gather:
●	Patients are identified by an SSN, and their names, addresses, and ages must be recorded.
●	Doctors are identified by an SSN. For each doctor, the name, specialty, and years of experience must be recorded.
●	Each pharmaceutical company is identified by name and has a phone number.
●	For each drug, the trade name and formula must be recorded. Each drug is sold by a given pharmaceutical company, and the trade name identifies a drug uniquely from among the products of that company. If a pharmaceutical company is deleted, you need not keep track of its products any longer.
●	Each pharmacy has a name, address, and phone number.
●	Every patient has a primary physician. Every doctor has at least one patient.
●	Each pharmacy sells several drugs and has a price for each. A drug could be sold at several pharmacies, and the price could vary from one pharmacy to another.
●	Doctors prescribe drugs for patients. A doctor could prescribe one or more drugs for several patients, and a patient could obtain prescriptions from several doctors.
●	Each prescription has a date and a quantity associated with it. You can assume that, if a doctor prescribes the same drug for the same patient more than once, only the last such prescription needs to be stored.
●	Pharmaceutical companies have long-term contracts with pharmacies. A pharmaceutical company can contract with several pharmacies, and a pharmacy can contract with several pharmaceutical companies. For each contract, you have to store a start date, an end date, and the text of the contract.
●	Pharmacies appoint a supervisor for each contract. There must always be a supervisor for each contract, but the contract supervisor can change over the lifetime of the contract.
Draw an ER diagram that captures the preceding information. Identify any constraints not captured by the ER diagram.
How would your design change if each drug must be sold at a fixed price by all pharmacies?
How would your design change if the design requirements change as follows: If a doctor prescribes the same drug for the same patient more than once, several such prescriptions may have to be stored?
### Answer:
![ERD]()
___
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
___
## [Lab: 06]()
### Exercise
Question 1
Insert the following data into the following table
	Movie (id, title, year, director)
|Id	 |Title	               |Year	|Director        |
|----|---------------------|--------|----------------|
|1	 |Ben hur	           |2016	|Thomas          |
|2	 |Get Smart	           |2012    |Richard Bell    |
|3	 |Spider Man	       |2009    |Tam Morry       |
|4	 |Batman V/S Super Man |2015	|Gerald Hond     |
#### Query:
```
CREATE DATABASE Lab_06

CREATE TABLE Movie (
	Id INT(10) NOT NULL,
	title VARCHAR(20),
	yearr INT(4) NOT NULL,
	director VARCHAR(20)
);

INSERT INTO Movie (Id, title, yearr, director)
VALUES (1, 'Ben hur', 2016, 'Thmos'),
       (2, 'Get Smart', 2012, 'Richard Bell'),
       (3, 'Spider Man', 2009, 'Tam Morry'),
       (4, 'Batman V/S Super Man', 2015, 'Gerald Hond');
```
### Output ScreenShots:
![Movie Table](https://github.com/H-R-S/DBMS-Manual/blob/main/Lab_06/ScreenShots/movie_table.PNG)
___
## [Lab: 07]()
### Exercise
Question 1

Grant all privilege to user which name Ali.
#### Answer:
```
GRANT ALL PREVILEGES ON *.* TO 'Ali' @ ' localhost' ;
```

Question 2

Grant only creates permission to user which name Fahad.
#### Answer:
```
GRANT CREATE ON *.* TO 'Fahad' @ localhost';
```
___
## [Lab: 08]()
### Exercise
|Emp_num   |Emp_Name     |Emp_Job         |Emp_Sal     |
|----------|-------------|----------------|------------|
|E101	   |Salman	     |Analyst	      |6000        |
|E102	   |Bushra	     |Programmer	  |5000        |
|E103	   |Madiha	     |Web Designer	  |6000        |
|E104	   |Batool	     |ERD designer	  |4000        |
|E105	   |Hameed	     |Web Designer	  |3000        |
|E106	   |Nini	     |Analyst	      |2500        |
|E107	   |Imtiaz	     |Web Designer	  |6500        |
|E108	   |Rashid	     |Programmer	  |4000        |
|E109	   |Muzzamil	 |ERD designer	  |2000        |

1.	List all employees’ number, employee’s name and jobs from emp.
2.	List all employees’ number, employee’s name and jobs from emp whose salaries greater than 5,000.
3.	List all employees’ number, employee’s name and jobs from emp whose salaries less than 5,000.
4.	List all employees’ number, employee’s name and jobs from emp whose salaries between 1,000 to 5,000.
5.	List all employees’ number, employee’s name, jobs and salaries from emp.
#### Query:
```
CREATE DATABASE Lab_08

CREATE TABLE Employee (
	Emp_num VARCHAR(10) NOT NULL,
	Emp_Name CHAR(20),
	Emp_Job CHAR(20),
	Emp_Sal INT(10),
	PRIMARY KEY (Emp_num)
);

INSERT INTO Employee (Emp_num, Emp_Name, Emp_Job, Emp_Sal)
VALUES ('E101', 'Salman', 'Analyst', 6000),
       ('E102',	'Bushra', 'Programmer', 5000),
       ('E103', 'Madiha', 'Web Designer', 6000),
       ('E104',	'Batool', 'ERD designer', 4000),
       ('E105', 'Hameed', 'Web Designer', 3000),
       ('E106', 'Nini', 'Analyst', 2500),
       ('E107', 'Imtiaz', 'Web Designer', 6500),
       ('E108',	'Rashid', 'Programmer', 4000),
       ('E109', 'Muzzamil', 'ERD designer', 2000);
       
SELECT Emp_num, Emp_Name, Emp_Job FROM Employee;

SELECT Emp_num, Emp_Name, Emp_Job FROM Employee WHERE Emp_Sal > 5000;

SELECT Emp_num, Emp_Name, Emp_Job FROM Employee WHERE Emp_Sal < 5000;

SELECT Emp_num, Emp_Name, Emp_Job FROM Employee WHERE Emp_Sal BETWEEN 1000 AND 5000;

SELECT * FROM Employee;

```
### Output ScreenShots:
#### Question: 01
![Q1](https://github.com/H-R-S/DBMS-Manual/blob/main/Lab_08/ScreenShots/q1.PNG)
#### Question: 02
![Q2](https://github.com/H-R-S/DBMS-Manual/blob/main/Lab_08/ScreenShots/q2.PNG)
#### Question: 03
![Q3](https://github.com/H-R-S/DBMS-Manual/blob/main/Lab_08/ScreenShots/q3.PNG)
#### Question: 04
![Q4](https://github.com/H-R-S/DBMS-Manual/blob/main/Lab_08/ScreenShots/q4.PNG)
#### Question: 05
![Q5](https://github.com/H-R-S/DBMS-Manual/blob/main/Lab_08/ScreenShots/q5.PNG)
___
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
___
## [Lab: 10]()
### Exercise
Question No. 1
1.	List average salary of each job.
2.	Find average and sum of all the salaries of each job excluding clerks.
3.	Find average and sum of the salaries of each job excluding salesmen', clerk' and 'manager'.
4.	Find count, sum and average salaries of each job excluding salesmen', clerk' and 'manager'.
5.	List average salary of each department.
#### Query:
```
CREATE DATABASE Lab_10

CREATE TABLE Employee (
	Emp_num VARCHAR(10) NOT NULL,
	Emp_Name CHAR(20),
	Emp_Job CHAR(20),
	Emp_Sal INT(10),
	PRIMARY KEY (Emp_num)
);

INSERT INTO Employee (Emp_num, Emp_Name, Emp_Job, Emp_Sal)
VALUES ('E101', 'Salman', 'Analyst', 6000),
       ('E102',	'Bushra', 'Programmer', 5000),
       ('E103', 'Madiha', 'Web Designer', 6000),
       ('E104',	'Batool', 'ERD designer', 4000),
       ('E105', 'Hameed', 'Web Designer', 3000),
       ('E106', 'Nini', 'Analyst', 2500),
       ('E107',	'Ajmal', 'Clerk', 2000),
       ('E108', 'Imtiaz', 'Web Designer', 6500),
       ('E109',	'Rashid', 'Programmer', 4000),
       ('E110',	'Haris', 'Manager', 9000),
       ('E111', 'Muzzamil', 'ERD designer', 2000),
       ('E112',	'Rashid', 'Salesmen', 5000);
       
SELECT Emp_Job, AVG(Emp_Sal) FROM Employee GROUP BY Emp_Job;

SELECT Emp_Job, AVG(Emp_Sal), SUM(Emp_Sal) FROM Employee
WHERE Emp_Job <> 'Clerk' GROUP BY Emp_Job;

SELECT Emp_Job, AVG(Emp_Sal), SUM(Emp_Sal) FROM Employee
WHERE Emp_Job <> 'Salesmen' AND Emp_Job <> 'Clerk' AND Emp_Job <> 'Manager' 
GROUP BY Emp_Job;

SELECT COUNT(*), Emp_Job, SUM(Emp_Sal), AVG(Emp_Sal) FROM Employee
WHERE Emp_Job <> 'Salesmen' AND Emp_Job <> 'Clerk' AND Emp_Job <> 'Manager' 
GROUP BY Emp_Job;

SELECT Emp_Job, AVG(Emp_Sal) FROM Employee GROUP BY Emp_Job
```
### Output ScreenShots:
#### Question: 01
![Q1](https://github.com/H-R-S/DBMS-Manual/blob/main/Lab_10/ScreenShots/q1.PNG)
#### Question: 02
![Q2](https://github.com/H-R-S/DBMS-Manual/blob/main/Lab_10/ScreenShots/q2.PNG)
#### Question: 03
![Q3](https://github.com/H-R-S/DBMS-Manual/blob/main/Lab_10/ScreenShots/q3.PNG)
#### Question: 04
![Q4](https://github.com/H-R-S/DBMS-Manual/blob/main/Lab_10/ScreenShots/q4.PNG)
#### Question: 05
![Q5](https://github.com/H-R-S/DBMS-Manual/blob/main/Lab_10/ScreenShots/q5.PNG)
___
## [Lab: 11]()
### Exercise
Question No. 1
1.	Find the names of Top 10 employees which salaries are highest.
#### Query:
```
CREATE DATABASE Lab_11

CREATE TABLE Employee (
	Emp_num VARCHAR(10) NOT NULL,
	Emp_Name CHAR(20),
	Emp_Job CHAR(20),
	Emp_Sal INT(10),
	PRIMARY KEY (Emp_num)
);

INSERT INTO Employee (Emp_num, Emp_Name, Emp_Job, Emp_Sal)
VALUES ('E101', 'Salman', 'Analyst', 6000),
       ('E102',	'Bushra', 'Programmer', 5000),
       ('E103', 'Madiha', 'Web Designer', 6000),
       ('E104',	'Batool', 'ERD designer', 4000),
       ('E105', 'Hameed', 'Web Designer', 3000),
       ('E106', 'Nini', 'Analyst', 2500),
       ('E107', 'Imtiaz', 'Web Designer', 6500),
       ('E108',	'Rashid', 'Programmer', 4000),
       ('E109', 'Muzzamil', 'ERD designer', 2000);
       
SELECT * FROM Employee ORDER BY Emp_Sal DESC LIMIT 0,10
```
### Output ScreenShots:
![employee_table](https://github.com/H-R-S/DBMS-Manual/blob/main/Lab_11/ScreenShots/employee_table.PNG)
___
## [Lab: 12]()
### Exercise
1-Creates a stored procedure named "SelectAllCustomers" that selects all records from the "Customers" table.
2-creates a stored procedure that selects Customers from a particular City from the "Customers" table
3- Creates a stored procedure that selects Customers from a particular City with a particular PostalCode from the "Customers" table:
#### Query:
```
CREATE DATABASE Lab_12

CREATE TABLE Customers (
	customer_ID INT(10) NOT NULL PRIMARY KEY,
	fName CHAR(20),
	lName CHAR(20),
	address VARCHAR(50),
	city CHAR(20),
	postalCode VARCHAR(20),
	country CHAR(20)
);

INSERT INTO Customers(customer_ID, fName, lName, address, city, postalCode, country)
VALUES (1, 'Alfreds', 'Maria', 'Obere Str. 57', 'Berlin', '12209', 'Germany'),
       (2, 'Ana', 'Trujillo', 'Avda. de la Constitución 2222', 'México D.F.', '05021', 'Mexico'),
       (3, 'Antonio', 'Moreno', 'Mataderos 2312', 'México D.F.', '05023', 'Mexico'),
       (4, 'Thomas', 'Hardy', '120 HanoverSq.', 'London', 'WA1 1DP', 'UK'),
       (5, 'Berglunds', 'Christina', 'Berguvsvägen 8', 'Luleå', 'S-958 22', 'Sweden');
 
DELIMITER&& 
CREATE PROCEDURE SelectAllCustomers() 
BEGIN
	SELECT * FROM Customers;
END&& 
DELIMITER;

CALL SelectAllCustomers();

DELIMITER&& 
CREATE PROCEDURE CustomersFromParticularCity(IN particularCity CHAR(20))
BEGIN
	SELECT fName, city FROM Customers WHERE city = particularCity;
END&& 
DELIMITER;

CALL CustomersFromParticularCity('México D.F.');

DELIMITER&& 
CREATE PROCEDURE CustomersFromParticularCityWithParticularPostalCode(
IN particularCity CHAR(20), particularPostalCode VARCHAR(20))
BEGIN
	SELECT fName, city, postalCode FROM Customers 
	WHERE city = particularCity AND postalCode = particularPostalCode;
END&& 
DELIMITER;

CALL CustomersFromParticularCityWithParticularPostalCode('México D.F.', '05023');
```
### Output ScreenShots:
#### Question: 01
![Q1](https://github.com/H-R-S/DBMS-Manual/blob/main/Lab_12/ScreenShots/q1.PNG)
#### Question: 02
![Q2](https://github.com/H-R-S/DBMS-Manual/blob/main/Lab_12/ScreenShots/q2.PNG)
#### Question: 03
![Q3](https://github.com/H-R-S/DBMS-Manual/blob/main/Lab_12/ScreenShots/q3.PNG)
___