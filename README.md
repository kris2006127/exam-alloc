# exam-alloc
alloctation of rooms and seats to students

The Exam Allocation System is a DBMS mini project developed using Flask and MySQL. The system is designed to automate and manage exam hall allocation processes in educational institutions.

The project allows administrators to manage students, rooms, exams, and invigilators efficiently. A MySQL stored procedure is used to automatically allocate students to available exam rooms based on room capacity. The system also provides seating charts and room summaries for better exam management.

The backend is developed using Flask, while MySQL is used for database management. HTML templates are used to create the user interface.

Main Functionalities
Admin Login System
Student Management
Room Management
Exam Management
Automatic Seat Allocation
Seating Chart Generation
Room-wise Allocation Summary
Database Concepts Used
Primary Keys
Foreign Keys
Joins
Views
Stored Procedures
Constraints
Aggregate Functions

This project demonstrates the practical implementation of database concepts along with web application development using Python Flask and MySQL.


Technologies Used
Python
Flask
MySQL
HTML
Project Structure
exam_project/
│
├── app.py
├── db.py
├── exam_alloc.sql
│
└── templates/
    ├── login.html
    ├── dashboard.html
    └── students.html
Database Connection

Database connection is configured inside:

db.py

Example:

import mysql.connector


def get_db():

    return mysql.connector.connect(
        host="localhost",
        user="root",
        password="your_password",
        database="exam_alloc"
    )

To run the project on another computer, only change:

user="root"
password="your_password"

according to the MySQL username and password of that system.

Running the Project

Run the Flask application:

python app.py

Open browser:

http://127.0.0.1:5000
Default Login
Username: admin
Password: admin123
Main Modules
Login

Admin authentication using MySQL.

Students

Displays all student details.

Rooms

Displays room information and capacities.

Exams

Displays exam details.

Auto Allocation

Automatically allocates students to rooms using a MySQL stored procedure.

Seating Chart

Displays room-wise student seating arrangement.

Room Summary

Displays total students allocated in each room.

Database Concepts Used
Primary Keys
Foreign Keys
Joins
Views
Stored Procedures
Constraints
Author

Grisha V
