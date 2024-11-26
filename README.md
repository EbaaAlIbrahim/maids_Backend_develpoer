# Library Management System

This project is a Library Management System with RESTful APIs to handle book and patron management, as well as borrowing operations. It is built using Java, Spring Boot, and MySQL.

---

## Project Structure

- **`controller`**: Handles API requests (`BookController`, `BorrowingController`, `PatronController`).
- **`entity`**: Defines the data models (`Book`, `BorrowingRecord`, `Patron`).
- **`repository`**: Manages database interactions.
- **`service`**: Contains business logic for managing books, patrons, and borrowing.

- Base URL

http://localhost:8080/api
1. Book Management
GET /books: Retrieve all books.
GET /books/{id}: Retrieve details of a specific book by ID.
POST /books: Add a new book.
PUT /books/{id}: Update a book's information.
DELETE /books/{id}: Remove a book.
2. Patron Management
GET /patrons: Retrieve all patrons.
GET /patrons/{id}: Retrieve a specific patron by ID.
POST /patrons: Add a new patron.
PUT /patrons/{id}: Update a patron's information.
DELETE /patrons/{id}: Remove a patron.
3. Borrowing Management
POST /borrow/{bookId}/patron/{patronId}: Borrow a book.
PUT /borrow/return/{bookId}/patron/{patronId}: Return a book.
