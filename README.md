# Employee Management REST API

A backend REST API for managing employee records, featuring **CRUD operations** (Create, Read, Update, Delete).  
Built using **Spring Boot** with Java and tested thoroughly using **Postman**.

## 🚀 Features
- Add new employees (POST)
- Fetch all employees or by ID (GET)
- Update employee details (PUT)
- Delete employees (DELETE)
- RESTful API design
- Easy to extend for real-world use cases

## 🛠 Tech Stack
- **Java 17+**
- **Spring Boot** (Spring Web, Spring Data JPA)
- **H2 / MySQL** (configurable)
- **Postman** for API testing

## 📂 Project Structure
```plaintext
src/main/java/com/example/employee
├── controller       ⚡ REST controllers
├── model            🗂 Employee entity
├── repository       🗄 Data access layer
├── service          🔧 Business logic
└── EmployeeApplication.java
```

## 🔌 API Endpoints

### 1️⃣ Get All Employees
**GET** `/api/employees`  
Response:
```json
[
  {
    "id": 1,
    "name": "John Doe",
    "role": "Developer",
    "salary": 50000
  }
]
```
### 2️⃣ Get Employee by ID
**GET** `/api/employees/{id}`

### 3️⃣ Create New Employee
**POST** `/api/employees`
Response:
```json
{
  "name": "Alice Smith",
  "role": "Manager",
  "salary": 65000
}
```
### 4️⃣ Update Employee
PUT `/api/employees/{id}`
Body:
```json
{
  "name": "Alice Smith",
  "role": "Senior Manager",
  "salary": 75000
}
```
### 5️⃣ Delete Employee
DELETE `/api/employees/{id}`
## ⚡ How to Run Locally

## Clone the repository
```bash
git clone https://github.com/your-username/employee-management-api.git
cd employee-management-api
```
- **Open the project in your IDE (IntelliJ / Eclipse)**
- **Configure application.properties (optional if using MySQL)**
- **Run the Spring Boot application**

`mvn spring-boot:run`





