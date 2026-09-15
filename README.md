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
