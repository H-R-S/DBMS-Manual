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
![Movie Table]()