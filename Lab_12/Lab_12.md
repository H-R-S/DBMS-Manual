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
