# Employee Database Management System

## **Description**
The Employee Database Management System is a Java application that provides a way to manage employee data stored in a relational database. It allows users to perform **CRUD** (Create, Read, Update, Delete) operations on an `employee` table using **JDBC**. This project demonstrates the integration of Java with a MySQL database to manage employee records effectively.

---

## **Features**
- Create new employee records.
- Retrieve employee details by ID.
- Retrieve all employee records.
- Update employee information.
- Delete employee records from the database.

---

## **Technologies Used**
- **Java**: Programming language used for building the application.
- **JDBC**: Java Database Connectivity API for database interactions.
- **MySQL**: Relational database for storing employee data.
- **Maven**: Build automation tool for managing dependencies and project structure.

---

## **Database Schema**
The `employee` table in the database has the following structure:
| Column       | Type              | Description                      |
|--------------|-------------------|----------------------------------|
| `id`         | INT (Primary Key) | Auto-incremented employee ID.    |
| `name`       | VARCHAR(100)      | Employee name.                   |
| `position`   | VARCHAR(100)      | Employee's job position.         |
| `salary`     | DOUBLE            | Employee's salary.               |
| `hire_date`  | DATE              | Date of hiring.                  |

---

## **How to Run the Project**

### **1. Prerequisites**
- **Java JDK 11 or later** installed.
- **MySQL** database installed.
- **Maven** installed.
- A database named `employee_db` created in MySQL.

### **2. Database Setup**
1. Open your MySQL client (e.g., MySQL Workbench or CLI).
2. Execute the following SQL commands to set up the database and table:
   ```sql
   CREATE DATABASE employee_db;

   USE employee_db;

   CREATE TABLE employee (
       id INT AUTO_INCREMENT PRIMARY KEY,
       name VARCHAR(100) NOT NULL,
       position VARCHAR(100) NOT NULL,
       salary DOUBLE NOT NULL,
       hire_date DATE NOT NULL
   );
