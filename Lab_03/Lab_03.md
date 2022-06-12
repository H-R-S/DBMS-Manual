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
![Q1](https://github.com/H-R-S/DBMS-Manual/blob/main/Lab_03/ScreenShots/q1.png)

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
![Q2](https://github.com/H-R-S/DBMS-Manual/blob/main/Lab_03/ScreenShots/q2.png)