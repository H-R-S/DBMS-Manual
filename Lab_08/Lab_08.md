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
