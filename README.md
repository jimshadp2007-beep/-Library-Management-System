📚 Library Management System (SQL Project)
📌 Project Overview

The Library Management System is a database project developed using SQL.
It is designed to manage and maintain records of books, customers, employees, branches, and book transactions in a library.

The system keeps track of:

Books available in the library

Employees working in different branches

Customer registration details

Book issue and return records

Rental price and availability status of books

This project demonstrates the use of Relational Database concepts, including Primary Keys, Foreign Keys, Joins, Aggregate Functions, and SQL Queries.

🗄️ Database Name
library
🧩 Database Tables

The project contains 6 tables:

Table Name	Description
Branch	Stores information about library branches
Employee	Stores employee details working in branches
Books	Stores details about books in the library
Customer	Stores customer registration details
IssueStatus	Records details of books issued to customers
ReturnStatus	Records details of returned books
🏗️ Database Schema.


1️⃣ Branch
Column	Description
Branch_no (PK)	Unique branch number
Manager_Id	ID of the branch manager
Branch_address	Address of the branch
Contact_no	Contact number


2️⃣ Employee
Column	Description
Emp_Id (PK)	Employee ID
Emp_name	Employee name
Position	Job position
Salary	Employee salary
Branch_no (FK)	Branch reference


3️⃣ Books
Column	Description
ISBN (PK)	Unique book identifier
Book_title	Title of the book
Category	Book category
Rental_Price	Book rental price
Status	Availability status (Yes/No)
Author	Book author
Publisher	Book publisher


4️⃣ Customer
Column	Description
Customer_Id (PK)	Customer ID
Customer_name	Customer name
Customer_address	Customer address
Reg_date	Registration date


5️⃣ IssueStatus
Column	Description
Issue_Id (PK)	Issue record ID
Issued_cust (FK)	Customer who issued the book
Issued_book_name	Name of issued book
Issue_date	Date of issue
Isbn_book (FK)	Book ISBN


6️⃣ ReturnStatus
Column	Description
Return_Id (PK)	Return record ID
Return_cust	Customer returning the book
Return_book_name	Name of returned book
Return_date	Return date
Isbn_book2 (FK)	Book ISBN

🔍 SQL Queries Implemented

The project includes SQL queries for the following operations:

Retrieve available books with title, category, and rental price.

List employee names and salaries in descending order.

Display book titles along with customers who issued them.

Count total number of books in each category.

Retrieve employees earning more than ₹50,000.

List customers registered before 01-01-2022 who have not issued books.

Display branch numbers with the number of employees in each branch.

Find customers who issued books in June 2023.

Retrieve book titles containing the word "History".

Display branches having more than 5 employees.

Retrieve employees who manage branches and their branch addresses.

List customers who issued books with rental price greater than ₹25.

🛠️ Technologies Used

MySQL

SQL (DDL & DML)

GitHub for version control

▶️ How to Run the Project

Install MySQL / MySQL Workbench / phpMyAdmin

Create the database:

CREATE DATABASE library;
USE library;

Run the table creation SQL scripts.

Insert the sample data using the provided INSERT queries.

Execute the project queries.

Capture screenshots of the output for documentation.

📊 Project Output

Each SQL query produces a result showing:

Book availability

Customer book issue records

Employee salary information

Branch employee statistics

Book categories and counts

Screenshots of query outputs are included in the project documentation.

🎯 Learning Objectives

This project demonstrates:

Database Design

Relational Schema

Primary & Foreign Keys

SQL Joins

Aggregate Functions

Filtering with WHERE clauses

Grouping and Sorting data

👨‍💻 Author

jimshad 
