Todo API

This project is a simple Todo API built using .NET 8.0, ASP.NET Core Web API, and Entity Framework Core. It allows users to perform CRUD (Create, Read, Update, Delete) operations on Todo items.


How It Was Made

1. Project Setup

Created a new ASP.NET Core Web API project in Visual Studio 2022.

Targeted .NET 8.0.



2. Database Integration

Added and configured Entity Framework Core to use SQL Server.

Created a TodoContext class to manage database access.



3. Model Definition

Defined a TodoItem model with properties:

Id (unique identifier)

Title (task name)

Description (task details)

IsCompleted (status).




4. API Endpoints

Built a controller (TodoItemsController) to handle HTTP requests for CRUD operations:

GET: Retrieve all or a single Todo item.

POST: Add a new Todo item.

PUT: Update an existing Todo item.

DELETE: Remove a Todo item.




5. Database Configuration

Configured the database connection string in appsettings.json.

Used migrations to create the database schema.



6. API Documentation

Integrated Swagger UI for testing the API endpoints.




How It Works

1. Database
The application uses SQL Server as its database. The TodoContext class is responsible for managing the TodoItems table.


2. Endpoints

GET /api/TodoItems: Fetch all Todo items.

GET /api/TodoItems/{id}: Fetch a specific Todo item by ID.

POST /api/TodoItems: Add a new Todo item.

PUT /api/TodoItems/{id}: Update an existing Todo item.

DELETE /api/TodoItems/{id}: Delete a Todo item by ID.



3. Testing

Run the project in Visual Studio.

Open Swagger UI at https://localhost:<port>/swagger to test the endpoints.



This API serves as a simple example of building a RESTful service with .NET 8.0 and Entity Framework Core.

