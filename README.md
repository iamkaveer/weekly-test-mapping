# weekly-test-mapping
This project is a Java-based application developed using Spring Boot that demonstrates the implementation of different types of relationships between data models. The project includes four models - Student, Laptop, Course, and Book - and an embedded model called Address.

```diff
- DUE TO SOME TECHNICAL ISSUE, NOT ABLE TO RECORD VIDEO
```

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

#### Book
The Book model represents a book and includes the following fields:
1. ID: The unique identifier for the book.
2. title: The title of the book.
3. author: The author of the book.
4. description: The description of the book.
5. price: The price of the book.
6. student: A many-to-one relationship that represents the student who owns the book.

#### Address
The Address model is an embedded model that represents the address of a student and includes the following fields:
1. landmark: The landmark of the address.
2. zipcode: The zip code of the address.
3. district: The district of the address.
4. state: The state of the address.
5. country: The country of the address.

#### Endpoints
The following endpoints are available for each model:
Student Endpoints
1. GET /get-all-students: Retrieves a list of all students.
2. GET /get-students/{id}: Retrieves a specific student by ID.
3. POST /add-students: Creates a new student.
4. PUT /update-students/{id}: Updates an existing student by ID.
5. DELETE /delete-students/{id}: Deletes a specific student by ID.

Laptop Endpoints
1. GET /get-all-laptops: Retrieves a list of all laptops.
2. GET /get-laptops/{id}: Retrieves a specific laptop by ID.
3. POST /add-laptops: Creates a new laptop.
4. PUT /update-laptops/{id}: Updates an existing laptop by ID.
5. DELETE /delete-laptops/{id}: Deletes a specific laptop by ID.

Book Endpoints
1. GET /get-all-books: Retrieves a list of all Book.
2. GET /get-book/{id}: Retrieves a specific Book by ID.
3. POST /add-Book: Creates a new Book.
4. PUT /update-Book/{id}: Updates an existing Book by ID.
5. DELETE /delete-book/{id}: Deletes a specific Book by ID.

### Screenshots of Table

![Screenshot (74)](https://user-images.githubusercontent.com/41718548/221421846-503e5bb2-64e1-476c-8404-34cc51c69732.png)

![Screenshot (75)](https://user-images.githubusercontent.com/41718548/221421854-d86feef0-ea8b-4c01-9ea7-eb9b6b5d26ed.png)

![Screenshot (76)](https://user-images.githubusercontent.com/41718548/221421860-0bc6f79f-ae72-4810-9e28-3f9a887c5f72.png)

![Screenshot (77)](https://user-images.githubusercontent.com/41718548/221421863-02291d09-29f8-4913-b210-4c2b6daf7be1.png)

![Screenshot (73)](https://user-images.githubusercontent.com/41718548/221421867-b28c7589-b913-403b-81ee-21afd7445fb1.png)

### Screenshots of CRUD requests

![Screenshot (83)](https://user-images.githubusercontent.com/41718548/221421947-b49118e5-1fa1-45d8-a254-71fdff11a406.png)

![Screenshot (78)](https://user-images.githubusercontent.com/41718548/221421950-ff584543-5828-4fde-9daa-58b88cfeafef.png)

![Screenshot (79)](https://user-images.githubusercontent.com/41718548/221421953-14aa70a1-9213-4274-97ff-30eeeec789e8.png)

![Screenshot (80)](https://user-images.githubusercontent.com/41718548/221421960-3713b4a4-b36a-48c9-9755-21f3ebb9a864.png)

![Screenshot (81)](https://user-images.githubusercontent.com/41718548/221421963-54339f10-5a9f-4269-8d5f-aef8b383761a.png)

![Screenshot (82)](https://user-images.githubusercontent.com/41718548/221421939-2a5beae7-5541-4732-85f1-a926efd17771.png)
