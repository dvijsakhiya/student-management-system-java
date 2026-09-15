# student-management-system-java
A Java-based Student Management System developed using Java Swing, JDBC and Oracle Database. The application provides secure login and CRUD operations for student records, including adding, updating, searching, viewing and deleting student information through a user-friendly desktop interface.

# 🎓 AJP Student Management System

## 📌 Project Overview

AJP Student Management System is a Java-based desktop application developed to manage student records efficiently.

The application provides a graphical user interface using Java Swing and connects to an Oracle XE database using JDBC. It allows an authorized user to perform different operations on student records through a simple and user-friendly interface.

The system provides functionality to add, update, search, view and delete student information.

The main purpose of this project is to replace manual student record management with a computerized system that provides faster data entry, searching, updating and record management.

---

## 🎯 Objectives

The main objectives of the Student Management System are:

- To maintain student records digitally.
- To reduce manual record management.
- To provide easy student data entry.
- To search student records quickly.
- To update existing student information.
- To delete unwanted student records.
- To display all student records in tabular form.
- To provide login authentication.
- To connect the Java application with an Oracle database.
- To perform CRUD operations using JDBC.

---

# ✨ Features

## 🔐 Login Module

The application starts with a login screen.

The login page contains:

- Email field
- Password field
- Login button
- Cancel button

After successful login, the user is redirected to the Home Page.

If incorrect credentials are entered, the application displays an error message.

---

## 🏠 Home Page

The Home Page provides access to the major functions:

- Add Student
- Update Student
- Search Student
- View Student
- Delete Student
- Logout

This provides a central navigation point for the application.

---

## ➕ Add Student

The Add Student module allows the user to register a new student.

Student information includes:

- Enrollment Number
- Student Name
- Father Name
- City
- Branch
- Semester
- College Name

After entering the information, the user can click **Save** to store the record in the Oracle database.

---

## ✏️ Update Student

The Update Student module allows the user to modify an existing student record.

The user can:

1. Enter an enrollment number.
2. Search for the student.
3. Retrieve the existing information.
4. Modify the required details.
5. Click Update.

The updated information is stored in the database.

---

## 🔎 Search Student

The Search Student module allows the user to search for a student using the enrollment number.

After searching, the system retrieves information such as:

- Student Name
- Father Name
- City
- Branch
- Semester
- College Name

---

## 👁️ View Students

The View Student module displays student records in a table.

The application retrieves records from the database and displays them using a JTable.

The displayed information includes:

- Enrollment
- Name
- Father Name
- City
- Branch
- Semester
- College

---

## 🗑️ Delete Student

The Delete Student module allows the user to remove an existing student record.

The user can:

1. Enter the enrollment number.
2. Search the student.
3. Verify the information.
4. Delete the record.

The selected student record is removed from the database.

---

# 🔄 CRUD Operations

The project implements the four basic database operations:

### Create

Adding a new student record.

```text
INSERT

Read

Searching and viewing student records.

SELECT
Update

Changing existing student information.

UPDATE
Delete

Removing a student record.

DELETE

Therefore:

        STUDENT MANAGEMENT SYSTEM
                  |
        ┌─────────┼─────────┐
        ↓         ↓         ↓
      CREATE     READ      UPDATE
        |         |         |
      Add       Search     Edit
      Student   Student    Student
                  |
                  ↓
                DELETE
                  |
             Delete Student
💻 Technologies Used
Technology	Purpose
Java	Main programming language
Java Swing	Graphical User Interface
JDBC	Java-Database connectivity
Oracle Database XE	Database management
SQL	Database operations
NetBeans IDE	Project development
JTable	Displaying student records
JOptionPane	Messages and alerts
Oracle JDBC Driver	Connecting Java with Oracle
🏗️ System Architecture

The application follows a simple desktop application architecture:

             👤 USER
                |
                ↓
        ┌─────────────────┐
        │   Java Swing    │
        │  User Interface │
        └─────────────────┘
                |
                ↓
        ┌─────────────────┐
        │   Java Logic    │
        │   & JDBC        │
        └─────────────────┘
                |
                ↓
        ┌─────────────────┐
        │ Oracle Database │
        │     XE          │
        └─────────────────┘
                |
                ↓
        student_detail
🗄️ Database

The project uses an Oracle XE database.

The Java application connects to Oracle through JDBC.

The project contains a connection class:

Project/ConnectionProvider.java

The application uses the Oracle JDBC driver:

oracle.jdbc.driver.OracleDriver

The main student data table used by the application is:

student_detail
👨‍🎓 Student Information

The system manages the following student information:

Field	Description
Enrollment	Student enrollment number
Name	Student name
FName	Father's name
City	Student city
Branch	Engineering branch
Sem	Semester
CName	College name

Available branches include:

I.T
Mechanical
Chemical
Civil
ICT
Electrical
Auto Mobile
Computer

Available semesters:

1
2
3
4
5
6
⚙️ How the System Works
Step 1 – Start Application

The Java application starts with the Login window.

Step 2 – Login

The user enters email and password.

Step 3 – Home Page

After successful authentication, the Home Page opens.

Step 4 – Select Operation

The user can select:

Add
Update
Search
View
Delete
Logout
Step 5 – Database Operation

The selected operation is processed using Java and JDBC.

Step 6 – Oracle Database

The application communicates with the Oracle XE database.

Step 7 – Display Result

The result is displayed through the Java Swing interface.

🔐 Login Flow
       Start
         ↓
      Login
         ↓
 Enter Email & Password
         ↓
   Check Credentials
       /       \
     Valid     Invalid
      ↓          ↓
   Home Page   Error
      ↓
   Operations
🔄 Student Management Flow
                 Home
                   |
       ┌───────────┼───────────┐
       ↓           ↓           ↓
      Add       Search       View
       |           |           |
       ↓           ↓           ↓
    INSERT       SELECT      SELECT
       |           |           |
       └───────────┼───────────┘
                   |
             Student Records
                   |
             ┌─────┴─────┐
             ↓           ↓
           Update       Delete
             ↓           ↓
           UPDATE      DELETE
✅ Advantages
1. Easy Student Management

Student information can be managed from a single application.

2. Faster Searching

Students can be searched using their enrollment number.

3. Reduces Manual Work

Digital records reduce dependency on paper-based student records.

4. CRUD Operations

The application supports:

Create
Read
Update
Delete
5. User-Friendly Interface

Java Swing provides a graphical interface with buttons, text fields, tables and forms.

6. Centralized Data

Student records are stored in the Oracle database.

7. Easy Record Updating

Existing records can be modified without creating a new record.

8. Easy Record Deletion

Unwanted records can be removed from the database.

9. Database Connectivity

The application demonstrates practical use of JDBC with Oracle.

10. Useful Academic Project

The project demonstrates concepts of Java, Swing, JDBC, SQL and database management.

❌ Disadvantages / Limitations
1. Desktop Application

The application is designed as a desktop application rather than a web or mobile application.

2. Oracle Dependency

The application requires an Oracle XE database for its current database connection.

3. Local Database Configuration

The database connection must be configured correctly on the computer where the application is executed.

4. Limited User Roles

The current system provides a basic login mechanism rather than a complete role-based authentication system.

5. Limited Reporting

Advanced student reports, statistics and graphical dashboards are not included.

6. No Web Access

The current application cannot be accessed directly through a web browser.

7. Security Improvements

The login credentials and database configuration should be improved before production use.

8. Scalability

For a very large educational organization, the system would require additional architecture and optimization.

🚀 Future Enhancements

The project can be enhanced with:

🌐 Web-based version
📱 Android/mobile application
👥 Multiple user roles
🔐 Improved authentication
🔑 Password encryption
📊 Student statistics dashboard
📈 Graphical reports
📄 PDF student reports
📥 Excel export
📧 Email notifications
🔎 Advanced search filters
🎓 Course/subject management
📝 Attendance management
📚 Marks/result management
💰 Fee management
☁️ Cloud database
🔔 Notification system
📁 Project Structure
AJP-Student-Management-System/
│
├── build/
│   └── classes/
│
├── nbproject/
│   ├── build-impl.xml
│   ├── project.properties
│   ├── project.xml
│   └── ...
│
├── src/
│   ├── login.java
│   ├── login.form
│   │
│   ├── home.java
│   ├── home.form
│   │
│   ├── newStudent.java
│   ├── newStudent.form
│   │
│   ├── SearchStudent.java
│   ├── SearchStudent.form
│   │
│   ├── UpdateStudent.java
│   ├── UpdateStudent.form
│   │
│   ├── DeleteStudent.java
│   ├── DeleteStudent.form
│   │
│   ├── ViewStudent.java
│   ├── ViewStudent.form
│   │
│   └── Project/
│       └── ConnectionProvider.java
│
├── build.xml
└── manifest.mf
🛠️ Installation
Requirements
JDK
NetBeans IDE
Oracle Database XE
Oracle JDBC Driver
Windows/Linux system
Step 1

Install Java JDK.

Step 2

Install NetBeans IDE.

Step 3

Install Oracle Database XE.

Step 4

Create the required database and student_detail table.

Step 5

Configure the Oracle JDBC connection.

Step 6

Open the project in NetBeans.

Step 7

Add the required JDBC libraries.

Step 8

Build and run the project.

The main class is:

login
📌 Important Database Configuration

The current source code contains an Oracle connection similar to:

jdbc:oracle:thin:@localhost:1521:XE

The database connection is defined in:

src/Project/ConnectionProvider.java

Before sharing the repository publicly, remove or change any real database password from this file.

Do not publish real credentials on GitHub.

🎓 Academic Project

Project Name: Student Management System

Subject: Advanced Java Programming (AJP)

Platform: Java Desktop Application

Database: Oracle XE

IDE: NetBeans

Programming Language: Java

Connectivity: JDBC
