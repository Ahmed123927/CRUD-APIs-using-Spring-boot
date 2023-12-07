# CRUD Demo REST API

This project is a simple CRUD (Create, Read, Update, Delete) demo REST API using Spring Boot. It exposes endpoints to manage employee records.

## Getting Started

To run this application locally, you need to have Java and Maven installed on your machine.

bash
git clone https://github.com/Ahmed123927/cruddemo.git
cd cruddemo
mvn clean install
java -jar target/cruddemo-0.0.1-SNAPSHOT.jar

The application will start on http://localhost:8080.
Endpoints

The following endpoints are available:

    GET /api/employees: Retrieve all employees.
    GET /api/employees/{employeeId}: Retrieve a specific employee by ID.
    POST /api/employees: Add a new employee.
    PUT /api/employees: Update an existing employee.
    DELETE /api/employees/{employeeId}: Delete an employee by ID.

Usage

You can use tools like Postman or curl to interact with the API endpoints.
Examples:

    Retrieve all employees:

bash

curl http://localhost:8080/api/employees

    Retrieve a specific employee by ID:

bash

curl http://localhost:8080/api/employees/{employeeId}

    Add a new employee:

bash

curl -X POST -H "Content-Type: application/json" -d '{"firstName": "John", "lastName": "Doe", "email": "john.doe@example.com"}' http://localhost:8080/api/employees

    Update an existing employee:

bash

curl -X PUT -H "Content-Type: application/json" -d '{"id": 1, "firstName": "Updated", "lastName": "Employee", "email": "updated.employee@example.com"}' http://localhost:8080/api/employees

    Delete an employee by ID:

bash

curl -X DELETE http://localhost:8080/api/employees/{employeeId}

Contributing

Feel free to contribute to this project by opening issues or creating pull requests. Your feedback and suggestions are welcome!
