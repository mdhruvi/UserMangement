# User Management REST API

This project is a REST API built with Java 17 and Spring Boot, allowing you to manage user data with the following features:
- Create a new user
- List all users
- Get a single user by ID
- Update an existing user
- Delete an existing user

## Technologies Used
- Java 17
- Spring Boot
- Spring Data JPA
- MySQL (using XAMPP)
- Eclipse IDE
- Jakarta Persistence (`jakarta.persistence.Entity`)

## Prerequisites

Before you begin, ensure you have met the following requirements:

- Java 17 or newer installed
- Eclipse IDE installed
- XAMPP installed and running MySQL server
- Postman or any REST client (for testing the API)

## Setting up the Project

### Step 1: Create the Database
1. Open XAMPP and start the MySQL server.
2. Create a database named `user_management` in MySQL:
   ```sql
   CREATE DATABASE user_management;
3. Create the users table in MySQL
   ```sql
   USE user_management;

   CREATE TABLE users (
      id BIGINT AUTO_INCREMENT PRIMARY KEY,
      username VARCHAR(50) NOT NULL,
      first_name VARCHAR(50) NOT NULL,
      last_name VARCHAR(50) NOT NULL,
      email VARCHAR(100) NOT NULL,
      phone_number VARCHAR(20) NOT NULL
   );
   ```

### Step 2: Clone the Repository

Clone the repository to your local machine:

```bash
git clone https://github.com/UserManagement/UserManagementAPI.git
```

### Step 3: Run the Application

1. Open the project in Eclipse IDE.
2. Right-click on the UserManagementApiApplication.java file and select Run As > Spring Boot App.
3. The Spring Boot application will start on http://localhost:8080.
