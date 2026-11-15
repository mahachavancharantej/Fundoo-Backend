# Fundoo Notes – Backend Application

A secure and scalable Note Management REST API developed using **Java, Spring Boot, Spring Security, JWT, and MySQL**. The application allows users to create, organize, search, and manage notes with secure authentication and authorization.

## 🚀 Technologies Used

- **Language:** Java
- **Backend Framework:** Spring Boot
- **Security:** Spring Security, JWT Authentication
- **Database:** MySQL
- **ORM:** Spring Data JPA, Hibernate
- **API:** RESTful Web Services
- **Build Tool:** Maven
- **Testing:** Postman

## ✨ Features

### Authentication & Authorization
- User Registration
- User Login
- JWT-based Authentication
- Role-Based Authorization
- Secure API Endpoints

### Notes Management
- Create, Read, Update, and Delete Notes
- Search Notes
- Add Labels to Notes
- Set Reminders
- Pin and Unpin Notes
- Archive and Unarchive Notes
- Move Notes to Trash
- Restore or Permanently Delete Notes

## 🏗️ Project Architecture

The application follows a layered architecture:

```text
src/main/java
    └── com.fundoo
         ├── controller
         ├── service
         ├── repository
         ├── model
         ├── dto
         ├── config
         ├── security
         ├── exception
         └── FundooApplication.java
```

## ⚙️ Prerequisites

Make sure you have installed:

- Java 17 or above
- Maven
- MySQL Server
- IntelliJ IDEA / Eclipse
- Postman

## 🔧 Database Configuration

Create a MySQL database:

```sql
CREATE DATABASE fundoo_notes;
```

Configure your `application.properties`:

```properties
spring.datasource.url=jdbc:mysql://localhost:3306/fundoo_notes
spring.datasource.username=root
spring.datasource.password=YOUR_PASSWORD

spring.datasource.driver-class-name=com.mysql.cj.jdbc.Driver

spring.jpa.hibernate.ddl-auto=update
spring.jpa.show-sql=true
spring.jpa.properties.hibernate.dialect=org.hibernate.dialect.MySQLDialect

server.port=8080
```

Replace `YOUR_PASSWORD` with your MySQL password.

## ▶️ How to Run the Application

**1. Clone the repository**

```bash
git clone YOUR_GITHUB_REPOSITORY_URL
```

**2. Navigate to the project directory**

```bash
cd Fundoo-Backend
```

**3. Build the application**

```bash
mvn clean install
```

**4. Run the application**

```bash
mvn spring-boot:run
```

The application will start at:

```text
http://localhost:8080
```

## 🔐 API Testing

Use Postman to test the REST APIs.

| Module | Operations |
|---|---|
| User | Register, Login |
| Notes | Create, Get, Update, Delete |
| Labels | Add, Update, Delete |
| Reminders | Set and Manage |
| Archive | Archive and Unarchive |
| Trash | Move, Restore, Delete |
| Security | JWT Authentication |

For secured endpoints, include the JWT token in the Authorization header:

```text
Authorization: Bearer YOUR_JWT_TOKEN
```

## 🛡️ Security & Exception Handling

- JWT-based authentication for secure access.
- Spring Security for endpoint protection.
- Role-based authorization.
- DTO-based request and response handling.
- Input validation.
- Centralized global exception handling.

## 🎯 Key Learning Outcomes

- Building RESTful APIs using Spring Boot.
- Implementing authentication and authorization using Spring Security.
- Integrating MySQL using Spring Data JPA.
- Applying layered architecture and DTO patterns.
- Handling exceptions and validating API requests.
- Managing relational database operations.

## 👩‍💻 Author

**Mahachavan Charan Tej**

Java  Developer | Spring Boot | REST APIs | MySQL

---

⭐ If you find this project useful, consider giving it a star!
