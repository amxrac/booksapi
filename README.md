# Bookstore API
A simple .NET Web API for managing books.


## Features
- CRUD Operations: Create, read, update, and delete books.

- Swagger/OpenAPI: Interactive API testing UI.

- SQL Server Integration: Uses Entity Framework Core for database operations.


## Technologies Used

- .NET 8

- Entity Framework Core

- SQL Server

- Swagger/OpenAPI


## Setup Instructions
### Prerequisites
  - .NET SDK

  - SQL Server

  - IDE (e.g., Visual Studio, VS Code)


#### Installation
1. Clone the repository:
   ``` bash
   git clone https://github.com/amxrac/booksapi.git```
2. Update the connection string in appsettings.json:
   ```json
   "ConnectionStrings": {
    "BooksDB": "Data Source=localhost;Initial Catalog=BooksDB;Integrated Security=True;"
    }```
3. Run migrations:
   ```bash
   dotnet ef database update  ```
4. Start the API:
   ```bash
   dotnet run     ```


## API Endpoints

| Method | Endpoint         | Description                |
|--------|------------------|----------------------------|
| GET    | `/api/books`     | Get all books              |
| GET    | `/api/books/{id}`| Get a book by ID           |
| POST   | `/api/books`     | Create a new book          |
| PUT    | `/api/books/{id}`| Update a book by ID        |
| DELETE | `/api/books/{id}`| Delete a book by ID        |


## Sample Request body (POST/PUT)
```json
{ 
  "author": "The Sisters Brothers",
  "title": "Patrick deWitt", 
}
```

### Using Swagger/OpenAPI
- Access Swagger UI at https://localhost:5001/swagger after running the API.
- Test endpoints directly from your browser!
