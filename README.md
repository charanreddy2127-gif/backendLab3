# Backend Development Fundamentals - Lab Work

**Student Name:** YARAVA CHARAN TEJ REDDY  
**Course:** Backend Development Fundamentals  
**Institution:** Aurora Deemed to be University  
**Faculty:** Yugandhar
**Repository:** [https://github.com/charanreddy2127-gif/backendLab3](https://github.com/charanreddy2127-gif/backendLab3)

---

## Course Lab Index

| Lab Folder | Module / Topic | Status |
| :--- | :--- | :---: |
| `backendLab3/` | **Lab 3: REST API, CRUD Operations, Query Parameters, Validation and Debugging** | Completed |

---

## Overview

This repository contains the implementation of Lab 3 for Backend Development Fundamentals. The project focuses on developing a RESTful API using Node.js and Express.js with SQLite as the database.

The application provides a Book Management System that allows users to create, retrieve, update and delete book records. It also supports searching, sorting, filtering and pagination to retrieve book information efficiently.

The project demonstrates fundamental backend development concepts, including REST API design, database connectivity, SQL queries, request validation and error handling.

---

## Technologies Used

- **Node.js** – JavaScript runtime environment.
- **Express.js** – Backend web framework for creating REST APIs.
- **SQLite** – Lightweight relational database.
- **sqlite3** – SQLite database driver.
- **sqlite** – Promise-based SQLite interface.
- **JavaScript** – Programming language used for backend development.
- **Postman** – API testing and verification.

---

## Features

- **GET All Books:** Retrieve all books from the database.
- **GET Book by ID:** Retrieve a specific book using its ID.
- **POST Book:** Add new book records to the database.
- **PUT Book:** Update existing book information.
- **DELETE Book:** Remove a book from the database.
- **Search Functionality:** Search books using their titles.
- **Sorting:** Sort books by ID, title, author or price.
- **Price Filtering:** Filter books using minimum and maximum price.
- **Pagination:** Retrieve records using limit and offset.
- **Input Validation:** Validate user inputs before performing database operations.
- **Error Handling:** Handle invalid requests and missing records with appropriate HTTP status codes.

---

## API Endpoints

| HTTP Method | Endpoint | Description |
| :--- | :--- | :--- |
| GET | `/books` | Retrieve all books |
| GET | `/books/:bookId` | Retrieve a book by ID |
| POST | `/books` | Add a new book |
| PUT | `/books/:bookId` | Update an existing book |
| DELETE | `/books/:bookId` | Delete a book |

---

## Query Parameters

The GET `/books` endpoint supports the following query parameters:

| Parameter | Description |
| :--- | :--- |
| `search_q` | Search books by title |
| `order_by` | Sort by id, title, author or price |
| `order` | Sorting order (ASC or DESC) |
| `limit` | Number of records to retrieve |
| `offset` | Number of records to skip |
| `min_price` | Minimum book price |
| `max_price` | Maximum book price |

### Example API Requests

**1. Retrieve all books**
```http
GET /books
```

**2. Search books by title**
```http
GET /books?search_q=Harry
```

**3. Sort books by price**
```http
GET /books?order_by=price&order=ASC
```

**4. Filter books by price**
```http
GET /books?min_price=10&max_price=50
```

**5. Pagination**
```http
GET /books?limit=5&offset=0
```

---

## Database Structure

The project uses an SQLite database named `books.db`.

The database contains a table named `book` with the following columns:

| Column | Data Type | Description |
| :--- | :--- | :--- |
| `id` | INTEGER | Primary key with auto-increment |
| `title` | TEXT | Name of the book |
| `author` | TEXT | Author of the book |
| `price` | REAL | Price of the book |

The application automatically creates the book table if it does not exist and inserts sample book records when the table is empty.

---

## Project Structure

```text
backendLab3/
│
├── books.db
│
├── server.js
│
├── package.json
│
├── package-lock.json
│
├── .gitignore
│
├── Screenshot 2026-11-08 184910.png
├── Screenshot 2026-11-08 184925.png
├── Screenshot 2026-11-08 184930.png
├── Screenshot 2026-11-08 184933.png
├── Screenshot 2026-11-08 184937.png
├── Screenshot 2026-11-08 184940.png
├── Screenshot 2026-11-08 184945.png
├── Screenshot 2026-11-08 184949.png
└── Screenshot 2026-11-08 184951.png
```

---

## Installation and Setup

Follow these steps to run the project locally.

### Step 1: Clone the Repository

```bash
git clone https://github.com/charanreddy2127-gif/backendLab3.git
```

### Step 2: Navigate to the Project Folder

```bash
cd backendLab3
```

### Step 3: Install Dependencies

```bash
npm install
```

### Step 4: Start the Server

```bash
npm start
```

### Step 5: Access the API

Once the server starts successfully, open the following URL:

```text
http://localhost:3000/books
```

The API is now ready to receive requests through Postman or another API testing tool.

---

## Testing

The API endpoints can be tested using Postman.

The following operations can be verified:

- Retrieving all book records.
- Retrieving a specific book using its ID.
- Adding new book records.
- Updating existing book information.
- Deleting book records.
- Testing search, sorting, filtering and pagination.
- Checking input validation and error responses.

---

## Learning Outcomes

Through this lab, I gained practical experience in:

- Developing RESTful APIs using Express.js.
- Understanding HTTP methods and status codes.
- Connecting Node.js applications with SQLite databases.
- Performing CRUD operations using SQL queries.
- Implementing query parameters for searching and filtering.
- Applying input validation and error handling.
- Testing backend APIs using Postman.

---

## Conclusion

This lab helped me understand the fundamentals of backend development and REST API implementation. By building a Book Management API, I gained hands-on experience with Express.js, SQLite, database operations and API testing.

The project strengthened my understanding of how backend applications handle client requests, process data and communicate with databases.

---

## Author

**Yarava Charan Tej Reddy**

B.Tech – Computer Science and Engineering

Aurora Deemed University

**GitHub:** [charanreddy2127-gif](https://github.com/charanreddy2127-gif)
