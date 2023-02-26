# weekly-test-mapping
This project is a Java-based application developed using Spring Boot that demonstrates the implementation of different types of relationships between data models. The project includes four models - Student, Laptop, Course, and Book - and an embedded model called Address.

### Data Models
#### Student
The Student model represents a student and includes the following fields:
1. ID: The unique identifier for the student.
2. name: The name of the student.
3. age: The age of the student.
4. phoneNumber: The phone number of the student.
5. branch: The branch of the student.
6. department: The department of the student.
7. address: An embedded model that represents the address of the student.

#### Laptop
The Laptop model represents a laptop and includes the following fields:
1. ID: The unique identifier for the laptop.
2. name: The name of the laptop.
3. brand: The brand of the laptop.
4. price: The price of the laptop.
5. student: A one-to-one relationship that represents the student who owns the laptop.

#### Course
The Course model represents a course and includes the following fields:
1. ID: The unique identifier for the course.
2. title: The title of the course.
3. description: The description of the course.
4. duration: The duration of the course.
5. studentList: A many-to-many relationship that represents the list of students who are enrolled in the course.
Book
The Book model represents a book and includes the following fields:

ID: The unique identifier for the book.
title: The title of the book.
author: The author of the book.
description: The description of the book.
price: The price of the book.
student: A many-to-one relationship that represents the student who owns the book.
Address
The Address model is an embedded model that represents the address of a student and includes the following fields:

landmark: The landmark of the address.
zipcode: The zip code of the address.
district: The district of the address.
state: The state of the address.
country: The country of the address.
Endpoints
The following endpoints are available for each model:

Student Endpoints
GET /students: Retrieves a list of all students.
GET /students/{id}: Retrieves a specific student by ID.
POST /students: Creates a new student.
PUT /students/{id}: Updates an existing student by ID.
DELETE /students/{id}: Deletes a specific student by ID.
Laptop Endpoints
GET /laptops: Retrieves a list of all laptops.
GET /laptops/{id}: Retrieves a specific laptop by ID.
POST /laptops: Creates a new laptop.
PUT /laptops/{id}: Updates an existing laptop by ID.
DELETE /laptops/{id}: Deletes a specific laptop by ID.
