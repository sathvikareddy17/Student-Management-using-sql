Student Management System

Overview
This project provides a simple Student Management System implemented using SQL.
It includes tables for storing student information, courses, enrollments, assignments, and grades.
This README file contains the SQL code to create the necessary tables and populate them with sample data.

Tables
Students
StudentID: Integer (Primary Key)
FirstName: VARCHAR(50) NOT NULL
LastName: VARCHAR(50) NOT NULL
DateOfBirth: DATE
Email: VARCHAR(50) UNIQUE
PhoneNumber: VARCHAR(15)
Courses
CourseID: Integer (Primary Key)
CourseName: VARCHAR(50) NOT NULL
Instructor: VARCHAR(50)
Enrollments
EnrollmentID: Integer (Primary Key)
StudentID: Integer (Foreign Key)
CourseID: Integer (Foreign Key)
EnrollmentDate: DATE
Assignments
AssignmentID: Integer (Primary Key)
CourseID: Integer (Foreign Key)
AssignmentName: VARCHAR(50)
DueDate: DATE
Grades
GradeID: Integer (Primary Key)
StudentID: Integer (Foreign Key)
AssignmentID: Integer (Foreign Key)
Score: FLOAT
