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
