# Day 3 - Data Modeling

1. Difference Between App, Object, Record, and Field

## App
An App is a collection of related tools, tabs, and objects designed for a specific purpose.

Example:
College Management App.

## Object
An Object is like a database table that stores information.

Example:
Student, Faculty, Course.

## Record
A Record is a single entry inside an object.

Example:
A student named Rahul is one record inside the Student object.

## Field
A Field stores specific information inside a record.

Example:
Student Name, Email, Age.

2. Standard vs Custom Objects

## Standard Objects
Standard objects are already provided by Salesforce.

Examples:
Account, Contact, Opportunity.

## Custom Objects
Custom objects are created based on business needs.

Examples:
Student, Course, Department.

3. Your college Data Model

## Objects
- Student
- Faculty
- Course
- Department

# Relationships

## One-to-Many Relationships
- One Department can have many Students
- One Department can have many Faculty members
- One Faculty member can teach many Courses

## Lookup Relationships
- Student → Department
- Faculty → Department
- Course → Faculty

Lookup relationships are useful because objects can stay independent while still being connected.

# Simple Data Model Diagram

Department
│
├── Students
├── Faculty
│
└── Courses

4. Formula Fields

## 1. Full Name
Combines first name and last name automatically.

It saves time and avoids manual typing mistakes.

## 2. Remaining Seats
Calculates available seats in a course.

Formula:
Total Seats - Enrolled Students

It automatically updates whenever students join the course.

## 3. Percentage
Calculates student percentage from marks.

Formula:
(Obtained Marks / Total Marks) * 100

It helps avoid manual calculation errors.

5. Validation Rules

## 1. Email Cannot Be Empty

Missing contact information for students or faculty.

## 2. Student Age Cannot Be Negative

Invalid or unrealistic age values.

## 3. Course Seats Cannot Exceed Limit

Overbooking students into a course.

# Reflection

Companies need structured data because it keeps information organized, accurate, and easy to access. 
Random spreadsheets often create duplicate data, confusion, and mistakes.
Structured systems like Salesforce help teams work faster, track information properly, and make better business decisions.
<img width="275" height="323" alt="Screenshot 2026-05-12 114611" src="https://github.com/user-attachments/assets/c2e88125-401b-4231-b4fc-570772b2e1bf" />
<img width="958" height="533" alt="Screenshot 2026-05-12 114532" src="https://github.com/user-attachments/assets/78736688-6b31-428c-8b12-d8d606fb73ea" />
<img width="959" height="535" alt="Screenshot 2026-05-12 114518" src="https://github.com/user-attachments/assets/84daa14f-8752-48c0-8c44-5453d664b04f" />



