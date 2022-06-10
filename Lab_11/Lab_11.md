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
