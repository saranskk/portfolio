# Student Management System

This is a **Student Management System** developed using **Java**, **SQL**, and **JDBC** in the **Eclipse IDE**. It is a console-based application that allows basic CRUD operations (Create, Read, Update, Delete) on student records stored in a relational database.

## 👩‍💻 Developed By

**Saranya**

## 🧰 Technologies Used

- Java (JDK 8 or above)
- Eclipse IDE
- MySQL (or any other RDBMS)
- JDBC (Java Database Connectivity)

## 📦 Features

- Add a new student
- View all students
- Update student information
- Delete a student by ID
- Search student by ID

## 🗂️ Project Structure

StudentManagementSystem/
│
├── src/
│ └── com/studentmanagement/
│ ├── Main.java # Entry point of the application
│ ├── Student.java # Model class for student entity
│ ├── StudentDAO.java # Data Access Object for DB operations
│ └── DBConnection.java # Handles the database connection
│
├── lib/ # (Optional) External libraries like MySQL Connector JAR
│
├── README.md
└── SQL/
└── student_schema.sql # SQL script to create student table


## 🗃️ Database Setup

1. Create a database in MySQL:
    ```sql
    CREATE DATABASE student_db;
    USE student_db;

    CREATE TABLE students (
        id INT PRIMARY KEY AUTO_INCREMENT,
        name VARCHAR(100),
        age INT,
        department VARCHAR(100)
    );
    ```

2. Add your database credentials in `DBConnection.java`:
    ```java
    String url = "jdbc:mysql://localhost:3306/student_db";
    String username = "your_username";
    String password = "your_password";
    ```

3. Include the **MySQL Connector JAR** in your Eclipse project:
    - Download from [https://dev.mysql.com/downloads/connector/j/](https://dev.mysql.com/downloads/connector/j/)
    - Right-click project > Build Path > Configure Build Path > Add External JARs > Select the `.jar` file

## ▶️ How to Run

1. Import the project into Eclipse:
    - `File` > `Import` > `Existing Projects into Workspace`

2. Ensure the MySQL Connector JAR is in the build path.

3. Open `Main.java` and run the file.

## ✅ Sample Operations (CLI)



