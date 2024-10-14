# Backend User Management Service

## Overview
This project is a simple backend service for managing users, built using Java 17 with the Spring Boot framework. The REST API allows clients to perform standard CRUD (Create, Read, Update, Delete) operations on user data. The service uses a file-based H2 database to persist user information, ensuring that data is retained across application restarts.

## API Endpoints
The service exposes the following REST API endpoints:

- **POST /users**: Create a new user.
- **GET /users**: Retrieve a list of all users.
- **GET /users/{id}**: Retrieve a single user by ID.
- **PUT /users/{id}**: Update an existing user's details.
- **DELETE /users/{id}**: Delete an existing user by ID.

## Technologies Used
- **Java 17**: The project is implemented using Java 17.
- **Spring Boot**: A framework for building Java-based enterprise applications.
- **Spring Data JPA**: Used for interacting with the H2 database.
- **H2 Database**: A file-based H2 database is used to persist user data across restarts.
- **Lombok**: Simplifies boilerplate code using annotations.

## Running the Application
To run the application locally, follow these steps:

1. **Clone the Repository**:
   ```
   git clone <repository-url>
   ```
2. **Navigate to the Project Directory**:
   ```
   cd backend
   ```
3. **Build and Run the Application**:
   ```
   ./mvnw spring-boot:run
   ```

## Accessing the H2 Console
The application uses a file-based H2 database. You can access the H2 console in your browser at:

- URL: `http://localhost:8080/h2-console`
- JDBC URL: `jdbc:h2:file:./data/testdb`
- Username: `sa`
- Password: `password`

**Note**: The file-based H2 database ensures persistence across restarts, and the repository may contain some test records already populated.



