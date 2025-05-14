# Employee Management System

This is a simple **Employee Management System** built using **Spring Boot** and **Maven**. It demonstrates basic CRUD operations for managing employee data.

## Features

- Add, view, update, and delete employees.
- RESTful API structure.
- Spring Data JPA with embedded H2/PostgreSQL (depending on configuration).

## Technologies Used

- Java
- Spring Boot
- Spring Data JPA
- Maven
- H2 / PostgreSQL (configure via `application.properties`)

## Getting Started

### Prerequisites

Make sure you have the following installed:
- Java 11+
- Maven 3+

### Setup & Run

1. **Clone the repository**:
   ```bash
   git clone https://github.com/yourusername/employee-management-system.git
   cd employee-management-system/employeemanagement
   ```

2. **Build the project**:
   ```bash
   ./mvnw clean install
   ```

3. **Run the application**:
   ```bash
   ./mvnw spring-boot:run
   ```

4. **Access the app**:
   - API base URL: `http://localhost:8080/api/employees`

### API Endpoints

| Method | Endpoint                | Description             |
|--------|-------------------------|-------------------------|
| GET    | `/api/employees`        | List all employees      |
| GET    | `/api/employees/{id}`   | Get employee by ID      |
| POST   | `/api/employees`        | Add new employee        |
| PUT    | `/api/employees/{id}`   | Update existing employee|
| DELETE | `/api/employees/{id}`   | Delete employee         |

## Project Structure

```
employeemanagement
├── controller/       # REST controllers
├── model/            # Entity classes
├── repository/       # Spring Data JPA Repositories
├── resources/
│   └── application.properties
├── EmployeemanagementApplication.java
└── pom.xml
```

## License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.
