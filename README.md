# CSE210-LabPerformance04-DCLP1-Constraints
MySQL database project implementing constraints (PK, FK, NOT NULL, UNIQUE, CHECK, ENUM) for Lab Performance 04 - CSE210
👨‍🎓 Student Information

Name: Your Name

ID: Your ID

Course: CSE210

Section: 242D3

Lab Performance: 04

Topic: DCLP1 – Constraints Implementation

📌 Project Overview

This project implements the given ERD in MySQL.
The following tables are created with proper constraints:

COUNTRY

DEPARTMENT

EMPLOYEE

FOLDER

The project includes:

Primary Keys (PK)

Foreign Keys (FK)

NOT NULL constraints

UNIQUE constraint

CHECK constraint

ENUM constraint

5 records inserted in each table

🗂 Database Name
company_db
🏗 Tables and Relationships
1️⃣ COUNTRY

country_id (PK)

country_name (UNIQUE, NOT NULL)

region (CHECK constraint)

2️⃣ DEPARTMENT

department_id (PK)

department_name (UNIQUE, NOT NULL)

country_id (FK → COUNTRY)

3️⃣ EMPLOYEE

employee_id (PK)

first_name (NOT NULL)

last_name (NOT NULL)

email (UNIQUE, NOT NULL)

salary (CHECK > 0)

gender (ENUM)

department_id (FK → DEPARTMENT)

4️⃣ FOLDER

folder_id (PK)

folder_name

created_date

employee_id (FK → EMPLOYEE)

UNIQUE (folder_name, employee_id)

🔑 Constraints Used

PRIMARY KEY

FOREIGN KEY

NOT NULL

UNIQUE

CHECK

ENUM

🧪 Sample Queries Used
Describe Tables
DESCRIBE COUNTRY;
DESCRIBE DEPARTMENT;
DESCRIBE EMPLOYEE;
DESCRIBE FOLDER;
View Data
SELECT * FROM COUNTRY;
SELECT * FROM DEPARTMENT;
SELECT * FROM EMPLOYEE;
SELECT * FROM FOLDER;
📸 Output

Screenshots of:

Table structure (DESCRIBE)

Inserted data (SELECT *)
are included in the submitted PDF file.

🔗 GitHub Repository Link

👉 Paste your GitHub repository link here

Example:

https://github.com/yourusername/DCLP1-Constraints
▶️ How to Run the Project

Open MySQL Workbench

Create a new database:

CREATE DATABASE company_db;
USE company_db;

Run the provided SQL script

Execute DESCRIBE and SELECT queries

Verify the inserted records

✅ Conclusion

This project successfully demonstrates the implementation of database constraints in MySQL according to the provided ERD. All tables were created with proper relationships and integrity rules.
