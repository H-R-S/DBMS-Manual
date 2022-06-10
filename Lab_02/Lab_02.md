## [Lab: 02]()
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